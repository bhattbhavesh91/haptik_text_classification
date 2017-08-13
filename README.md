# Classification of Haptik user queries into right Business Verticals using NLP and ML techniques.
Based on the Haptik user’s chat conversation, classify it into the right business vertical and assist the user with the requested services.

## Description:
Users often visit the chatbot system with a desire that the system will take action to help themselves on a certain request. To provide accurate support, the chatbot needs to determine the intent of the user. User intent detection will determine how the conversation between the user and the chatbot will take place. Therefore, if the user intent is misinterpreted, chatbot will give incorrect responses. At that time, the user may feel disgusted and have no intention of using the system again. The problem of detecting user intent is therefore very important in the chatbot system.

For Haptik, the number of user intentions are limited to a finite set of defined intents, which are related to the business operations that Haptik supports. So, the problem of detecting user intents can be formalized as the text categorization problem. With input being a text based request from the user, the classification system determines the intent corresponding to that saying from the set of intents that have been defined.

To build an intent classification model, we need a training dataset that includes different expressions for each intent. For example, with the same question about the weather in Mumbai today, users can use the following expressions:
 - What is the weather today in Mumbai?
 - Does Mumbai rain today?
 - What is the temperature in Mumbai today?
 - Excuse me, when going out today should we bring a raincoat?

It can be said that the training step for the intent classification problem is one of the most important tasks in developing the chatbot system, and it has a huge impact on the quality of the chatbot system. 
The first level Classifier needs to classify the conversation in the below mentioned domains:
- Travel - Flights
- Travel - Cabs
- Travel - Trains
- Nearby
- Recharge and Bills
- Reminders
- Food
- Movies
- home services

Sometimes, a user query may belong to multiple domains. (Ex. “Are there any offers going on?” This query could belong to all the domains in which transactions are possible ( travel, recharge, food, movies, home services, etc)

Formal Problem Statement and Datasets: 
A dataset containing user queries is provided. Each query is tagged by humans with single/multiple (all the applicable domains) domains. The task is to build a multi-label classifier using this training data. The classifier should tag all the possible domains for each query.

### Classes:
food, support(home services), reminders, movies, nearby, travel, recharge, casual, other
### Evaluation Criteria: 
There are two evaluation metric for this assignment
1: Classwise(k) precision and recall (True: class k is identified correctly)
2: Overall accuracy (True: All the classes are correctly identified for given record)


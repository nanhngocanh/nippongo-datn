
# NipponGo! - Japanese Communication Learning Website

## Overview
This is a project to develop a website that supports learners in Japanese communication, featuring the following functions:

* **Learning and Testing**: Provides communication knowledge.
* **Flashcards**: Offers an easy-to-remember vocabulary learning method.
* **Practice with Peers**: Creates a practice environment for learners by pairing and chatting one-on-one with any peer anonymously.
* **Practice with the App**: Provides practice scenarios with role-playing together with a chatbot.
## Architecture
The project is developed based on a microservice architecture, consisting of the following main components:

![image](https://github.com/nanhngocanh/nippongo-datn/assets/86515768/eeee0d9a-4caf-45fa-9c87-4a02e0005657)


### Keycloak: 
Authentication platform.
* Deployment link: https://35.247.160.15:8443/
### LearningService: 
Includes functions related to lessons and tests.
* Framework: [Spring Boot](https://spring.io/projects/spring-boot)
* Deployment link: https://35.247.160.15:8002/
* Github: [nihongo-be](https://github.com/nanhngocanh/nihongo-be)
### FlashcardService: 
Includes functions for managing flashcards.
* Framework: [Spring Boot](https://spring.io/projects/spring-boot)
* Deployment link: https://35.247.160.15:8001/
* Github: [flashcard-be](https://github.com/nanhngocanh/flashcard-be)
### ChatRoomMatcher: 
Responsible for pairing two users in an online video chat room via P2P identification.
* Framework: [Spring Boot](https://spring.io/projects/spring-boot)
* Deployment link: https://35.247.160.15:8003/
* Github: [chat-room-matcher](https://github.com/nanhngocanh/chat-room-matcher)
### ChatbotService: 
Automated chatting with users.
* Framework: Spring Boot
* Deployment link: updating...
* Github: updating...
### Front-end: 
End-user interface.
* Framework: [Angular](https://angular.io)
* Deployment link: https://nanhngocanh.github.io/nihongo/
* Github: [nihongo](https://github.com/nanhngocanh/nihongo)
### Kong API Gateway: 
https://35.247.160.15:9443/
* LearningService: **/learning-service**
* FlashcardService: **/flashcard-service**
* ChatRoomMatcher: **/chat-room-matcher**
* Chatbot: **/chatbot**

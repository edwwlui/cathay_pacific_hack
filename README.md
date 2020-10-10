Codebase for team MachineLearning in Cathay Pacific Hackathon '18. 

This project implements a custom chatbot "Anita" on Facebook Messenger that engages Cathay Pacific's passengers by providing personalized information about available in-flight services like on-flight Wifi, seat upgrades, etc. 
Anita will increase passengers' awareness of in-flight services available to them and consequently will increase Cathay Pacific's in-flight sales, all with a fairly low-cost chatbot solution. 

Facebook Messenger is used on the front-end while DialogText, a Google-owned NLP processor, implements the back-end. 

The files in this repository set up a local web server, exposes the server to the web using another proxy server and takes care of message processing between Facebook Messenger and Dialogflow.

index.js sets up the local server for "listening" for messages sent to the chatbot. 

process-message.js passes a user response from Facebook Messenger to DialogFlow and returns the chatbot's corresponding response according to DialogText back to Facebook. 

message-webhook.js enables Dialogflow to receive Facebook messages.

verify-webhook.js connects Facebook and the local server and conducts a security check between them.
# APIs with Lambda + API Gateway

**Author:** Caelan Dever  
**Email:** caelanwd@gmail.com

---

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_c9d0e1f2)

---

## Introducing Today's Project!

In this project, I will demonstrate how to build an API without having to manage traditional servers I'm doing this project to learn Lambda and API Gateway.

### Tools and concepts

Services I used were AWS Lambda and API Gateway service. Key concepts I learnt include Lambda functions, how to set up API Gateways, and API specification types.

### Project reflection

This project took me approximately 55 minutes. The most challenging part was publishing my API documentations. It was most rewarding to be able to write and publish my own API documentation. 

Why did you do this project today? Did this project meet your goals?

I did this project to add more hands on skills to my use of AWS Lambda and API gateways and the project definately did. 

---

## Lambda functions

AWS Lambda is a service that lets you run code without needing to manage any computers/servers - Lambda will manage them for you. I'm using Lambda in this project to build an API without having to manage traditional servers. 

The code I added to my function will set up a Lambda function that retrieves data from a DynamoDB table.

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_a1b2c3d5)

---

## API Gateway

APIs are like a messenger that carries requests and responses between systems. There are different types of APIs, like REST, HTTP, and WebSocket. My API is a REST API

Amazon API Gateway is the "front door" to our Lambda function. I'm using API Gateway in this project to receive requests and then forwards them to Lambda functions for processing. 

When a user makes a request Lambda processes the request, then sends the response through the API Gateway back to the user.

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_m3n4o5p6)

---

## API Resources and Methods

An API is made up of resources, which are individual endpoints within your API that handle different parts of its functionality.

Each resource consists of methods, which are based on standard HTTP methods, which are different commands that let you interact with data over the internet. For example:





GET to retrieve,



POST to add,



PUT to update, and



DELETE to remove 

I created a Lambda proxy integration. API Gateway doesn't need to reformat the user's request. Instead, it passes the entire request—headers, query parameters, path parameters, and body directly to Lambda. 

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_c9d0e1f2)

---

## API Deployment

When you deploy an API, you deploy it to a specific stage. A stage is  is a snapshot of your API at a specific point in time. I deployed to production, the live environment where your API is fully working, and there is live traffic and real users.

To visit my API, I put the invoke URL in a new tab search bar.  The API displayed an error because we haven't set up our DynamoDB table yet.

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_3ethryj2)

---

## API Documentation

For my project's extension, I am writing API documentation because it is a detailed description of an API's functionality. You can do this in the section dedicated to API: UserRequestAPI.

Once I prepared my documentation, I can publish it to the prod stage. You have to publish your API to a specific stage because it makes sure  that your documentation is consistent with the API version deployed to that stage.

My published and downloaded documentation showed me the main difference between the automatically generated documentation and the manually written part in your API is the level of customization and specificity in each section. 

![Image](http://learn.nextwork.org/happy_amber_shy_newt/uploads/aws-compute-api_z9a0b1c2)

---

---

# AWS: API, Dynamo and Lambda

## What is Amazon API Gateway?

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

## How does API Gateway work?

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct back ends.

API Gateway integrates with many other AWS services like AWS Lambda, AWS SNS, AWS IAM, and Cognito Identity Pools.

## Why is API Gateway an essential part of the Serverless ecosystem?

Within the Serverless ecosystem, API Gateway is the piece that ties together Serverless functions and API definitions.

## How does API Gateway integrate with other AWS services?

Many AWS services support integration with Amazon API Gateway, including:

1. AWS Lambda:

run Lambda functions to generate HTTP API responses.

2. AWS SNS:

publish SNS notifications when an HTTP API endpoint is accessed.

3. 

Amazon Cognito: provide authentication and authorization for your HTTP APIs.

## Framework?

The Serverless Framework uses a Lambda Proxy integration to make API Gateway events easily available to your Serverless functions.

## API Types

1. RESTful APIs

Build RESTful APIs optimized for serverless workloads and HTTP back ends using HTTP APIs

2. WEBSOCKET APIs

Build real-time two-way communication applications, such as chat apps and streaming dashboards, with WebSocket APIs.

## benefits

1. Efficient API development :

Run multiple versions of the same API simultaneously with API Gateway, allowing you to quickly iterate, test, and release new versions.

2. Performance at any scale :

Provide end users with the lowest possible latency for API requests and responses by taking advantage of our global network of edge locations using Amazon CloudFront.

3. Cost savings at scale :

API Gateway provides a tiered pricing model for API requests.

4. Easy monitoring :

Monitor performance metrics and information on API calls, data latency.

5. Flexible security controls :

Authorize access to your APIs with AWS Identity and Access Management and Amazon Cognito.

6. RESTful API options :

Create RESTful APIs using HTTP APIs or REST APIs.



# DYnamoDB

## what is the DYnamoDB ????

DynamoDB is a hosted NoSQL database offered by Amazon Web Services.

it offers :

1. reliable performance.

2. a managed experience.

3. simple API allowing for simple key-value access as well as more advanced query patterns.

## where to use it ???

1. Applications with large amounts of data and strict latency requirements.

2. Serverless applications using AWS Lambda.

3. Data sets with simple, known access patterns.
4. 

## Amazon DynamoDB??

Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale.

1. It's a fully managed.

2. multi-region.

3. multi-active.

4. durable database with built-in security.

5. backup and restore.

6. in-memory caching for internet-scale applications.

DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

## Benefits

1. Performance at scale

DynamoDB supports some of the world’s largest scale applications by providing consistent.

2. No servers to manage

DynamoDB is serverless with no servers to provision, patch, or manage and no software to install.

3. Enterprise ready

DynamoDB supports ACID transactions to enable you to build business-critical applications at scale.

## Applications

1. Serverless Web Apps

Build powerful web applications that automatically scale up and down.

2. Mobile Back ends

Use DynamoDB and AWS AppSync to build interactive mobile and web apps with real-time updates.

3. Microservices

Build flexible and reusable microservices using DynamoDB as a serverless data store for consistent and fast performance.

## Use cases

1. ad tech

2. gaming

3. Retail

4. Banking and Finance

5. Media and entertainment

6. Software and internet


# Description

Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.


## Key Features#

1. Type safety.

2. High level API

3. Easy to use syntax

4. Ability to transform data before saving or retrieving documents

5. Strict data modeling (validation, required attributes, and more)

6. Support for DynamoDB Transactions

7. Powerful Conditional/Filtering Support

8. Callback & Promise support
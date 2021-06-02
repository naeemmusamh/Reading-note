# AWS: Events


# SNS (Simple Notification Service)


SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients.

it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.

A distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS ,SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.

SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.


# SQS (Simple Queue Service)

SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages.

Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later.

SQS is mainly used to decouple applications or integrate applications. Messages can be stored in SQS for short duration of time.
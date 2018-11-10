## Inspiration
Single framework for translation, image detection, image search ,managing content in enterprise repository, and analysis of documents in the repository  just at your fingertips. also automatically finding text in the images so that we can translate text of the image also. Same framework serves product feedback analyse and creates a beautiful dashboards 

## What it does
It does almost everything what AWS AI framework provides.
### Translate Text,
### Find images in S3 bucket based on keyword,
### List face to create your own collection
### Search faces in the S3 bucket
### Search user by Name , User ID and Face
### Analysis of Product Feedback using Elastic Search and Kibana
### Provide dashboard which sentiments, keywords, ratings in customer feedback of produts

## How I built it

I learnt everything from AWS AI  libraries and utilized Amzon Lex bot framwework to create 'Turbo Mobile Bot'  for an enterprise called ' Turbo Mobile'. I integrated this bot with 'Slack' and Amazon ElasticSearch. Slack is the front end where all data of images, documents and product review are stored in S3 bucket. Whenever any item is uploaded in S3 bucket, event is triggered and based on type of uploaded file ( image, doc or feedback) details are logged on Elastic Search engine to create multiple indices. Elastic Search is interfaced with Kibana. Amazing and beautiful dashboards are created on Kibana for live analysis of images, documents and customer feedback.
Two different Lambda functions are used first to receive S3 trigger whenever item is  put in the bucket and second one is to fulfill intents from Lex bot

## Challenges I ran into
I got challenges in analyzing images, detecting input languages. Controlling the data flow in intents of Lex. But with practice, I got the right slot setting and data flow for Lex and then integrated Lex with Slack. To manage multiple intents was tedious because bot serves so many task in single lambda function

## Accomplishments that I'm proud of
I have learnt Amazon AI and ML libraries, it was fun integrating Lex with Slack and Kibana. I created my own search engine first time. I created an end to end solution.

## What I learned
All AI libraries, Lex, Slack, Kibana, ElasticSearch , EC2 , Kinesis oh so manythings

## What's next for Turbo Mobile Bot - enterprise bot based framework
Lot of stuff is pending, immediate next is to create image capturing prototype using Raspberry Pi and upload on S3 bucket to detect the person which shall be used for employee identification, Then live one to one audio translation
on mobile , live image translator on mobile, Hotword ( Wakeword) based apps and son on..........

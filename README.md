<img width="4014" height="207" alt="image" src="https://github.com/user-attachments/assets/b98e1317-f9c6-4acf-bb49-1148b2995309" />

## 🚀 BUILDING A SERVERLESS WEB APP 🚀

This repository shows how we can deploy a serverless webapp in Aws

## prerequisites
### Prerequisites
📌 AWS account

📌 Basic knowledge of Linux

📌 Python lamda

## ⚙️List of AWS services Used

-🌍 Amazon CloudFront

-🌐 Amazon Route 53

-💻 Amazon Lambda

-⚖️ Amazon s3

-🪪 Amazon Certificate Manager

-🗄️ Amazon Dynamo DB

-☁️ Amazon VPC

-🔐 Amazon WAF

-👁️ Amazon CloudWatch

-🌉 Amazon API Gateway


## 🤔 What is Serverless architecture
In the traditional server architecture you need to manage server maintaince , updates, os patching and everything in your server is maintained by you. But serverless architecture demonstrates a modern, scalable web application built entirely on AWS managed services, eliminating the need for server management. Serverless architecture means building and running applications without managing servers. You still write code, but AWS handles the infrastructure—scaling, patching, provisioning—automatically.

## 🏠 Architecture
<img width="1548" height="475" alt="image" src="https://github.com/user-attachments/assets/4ffe28da-04a4-4eae-bef7-dad7e8a463e2" />

##steps

## 🔹Route 53
To  host our webapp we need a domain name. so in the aws domain registration we buy a domain name "coffeeshopbean.com". Route53 routes trsffic across the every edge locations in the world through the cloudfront.

<img width="1705" height="801" alt="image" src="https://github.com/user-attachments/assets/8a261216-b162-41a2-8397-0890ba3f3db6" />

## 🔹Cloudfront
Amazon CloudFront is a global content delivery network (CDN) service that significantly enhances the performance and reliability of web content delivery. It works by caching content in strategically located servers known as edge locations, which are distributed worldwide. When a user requests content, CloudFront routes the request to the nearest edge location, ensuring low latency and high transfer speeds. so we created a distribution for our domain in the cloudfront.

<img width="2812" height="1469" alt="Screenshot 2025-07-12 155341" src="https://github.com/user-attachments/assets/f28a0a39-a726-4ace-a768-da68956d9951" />

## 🔹Amazon certificate Manager

we need secure our application outside of aws mean in the internet. For this we request SSL/TLS certificate that routes our traffic in a secure network preventing from outsiders without exposing. we created a certificate for our domain in the AWS certificate manager.

<img width="1641" height="769" alt="image" src="https://github.com/user-attachments/assets/8912fe10-bbcb-4768-8718-0ecf793cd6ca" />

## 🔹Amazon Lambda
Lambda function is used to invoke a container for our application when request came. By using lambda we don't need to manage servers and there is auto scaling. In lambda there is pay-per-request pricing only.

<img width="1705" height="822" alt="image" src="https://github.com/user-attachments/assets/50164993-0117-4c8a-92db-2b5774c18723" />

## Amazon s3

The application files of our application will be stored in the s3 buckets in the form of objects.

<img width="1681" height="823" alt="image" src="https://github.com/user-attachments/assets/eed4ad32-26ee-4c55-8cee-3c6b0e8c21bc" />

## API Gateway
Api gateeway is used to trigger the lambda funtion and and handles requests and responses from the route53.This gateway invokes the lambda through the user request.

<img width="1694" height="831" alt="image" src="https://github.com/user-attachments/assets/268befde-d725-446f-96ce-3114ee4008d4" />


























# Automated-Blog-Generation-using-AWS-Bedrock

This project leverages AWS Bedrock, the Llama model, AWS Lambda functions, and an S3 bucket to automate blog generation. Postman is used to interact with the API.

Table of Contents
Environment Setup
[Environment Setup](#environment-setup)
Writing Code in AWS Lambda
Hitting API using Postman
Downloading Data from S3 Bucket
Environment Setup
Create an AWS Account:

Sign up at AWS.
Set up AWS CLI:

Install AWS CLI from here.
Configure AWS CLI with aws configure and provide your AWS Access Key ID and Secret Access Key.
Create S3 Bucket:

Go to the S3 console and create a new bucket (e.g., blog-generation-bucket).
Set up AWS Lambda:

Go to the Lambda console and create a new function.
Choose "Author from scratch" and provide a function name (e.g., BlogGeneratorFunction).
Set the runtime to Python 3.x.
Writing Code in AWS Lambda
Lambda Function Code:

Use the following sample code for your Lambda function:

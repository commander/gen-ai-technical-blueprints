# Modernize in-store operations with AI

## Business challenge

You’re a retailer who needs to digitize and streamline legacy, paper-based processes for store associates to improve productivity and customer service.

## Tech stack

1. Amazon Rekognition
2. AWS Lambda
3. Amazon DynamoDb
4. Amazon S3
5. AWS Amplify
6. Amazon API Gateway
7. Amazon Cognito
6. Amazon Elasticache (Redis)

## Blueprint
1. An associate uses a mobile device to scan a product self
2. Amazon Rekognition anlyzes the image to identify products and price tags
3. Application running on AWS Lambda (Or ECS Fargate or EKS) cross-references this with invetory data stored in DynamoDb or S3
4. The device displays inventory status, ordering needs, or planogram for compliance.
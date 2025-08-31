# Make it easy for users to find and discover unique items on your online site

## Business challenge

You have millions of unique, non-standard items needed to provide a highly relevant, fast, and personalized search experience for its users.

## Tech stack

1. Amazon S3
2. AWS Managed Services For Apache Flink
3. AWS Kinesis Data Stream
4. AWS EKS
5. AWS DynamoDb
6. AWS Sagemaker AI

## Blueprint
1. A seller lists a new item, and its data is stored in DynamoDb
2. Kinesis Data stream and Managed Service for Apache Flink processes item details and user interaction data in real-time
3. This data enriches search indexes and feeds machine learning models running on EKS
4. The machine learning models are trained using Sagemaker AI
5. When a user searches, the models provide personalized rankings, which are served in milliseconds.
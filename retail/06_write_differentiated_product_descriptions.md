# Write differentiated product descriptions 

## Business challenge
You’re a large e-commerce retailer that needs to create unique, high-quality, and SEO-friendly product descriptions for thousands of items at scale, reducing manual effort and avoiding duplicate content.

## Tech stack
1. Amazon Bedrock or Sagemake AI
2. AWS Lambda or ECS Fargate
3. Amazon Redshift or Athena + S3

## Blueprint
1. A merchandiser inputs key product attributes (e.g., material, color, target audience) into a product management tool (Hosted on EC2 or AWS Amplify)
2. These attributes are sent to a service on AWS Lambda or ECS Fargate
3. The service constructs a detailed prompt and calls the Amazon Bedrock API
4. Amazon Bedrock API analyzes the attributes and returns multiple unique description options 
5. The descriptions are displayed to the merchandiser for review, editing, and final approval.
6. Approved descriptions and performance metrics are logged into Amazon Redshift or S3 and queried via Amazon Athena.
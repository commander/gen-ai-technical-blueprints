# Give your store managers ways to see real-time inventory

## Business challenge

You want to boost efficiency by giving your store managers accurate, real-time inventory recommendations.

## Tech stack
1. AWS Elastic Kubernetes Service (EKS)
    - AWS Fargate or EC2 With Autoscaling as alternative
2. AWS Athena + AWS S3
3. CloudFront
4. API Gateway
5. AWS DynamoDb

## Blueprint
1. Daily sales and inventory data from thousands of stores is ingested into Athena
2. Sagemaker models process historical data to predict demand for each item
3. QuickSights generates dashboards with recommended stock levels
2. Store associates' can view the dashboards on the mobile app.



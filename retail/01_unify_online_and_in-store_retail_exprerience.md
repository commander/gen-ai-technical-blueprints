# Unify online and in-store retail experiences

## Business challenge

You're a large retailer with valuable physical stores and a growing e-commerce channel. These two worlds operate in silos, creating a disconnected experience where customers face inconsistent pricing, promotions, and inventory levels.

## Tech stack
1. AWS Elastic Kubernetes Service (EKS)
    - AWS Fargate or EC2 With Autoscaling as alternative
2. AWS Athena + AWS S3
3. CloudFront
4. API Gateway
5. AWS DynamoDb + Lambda

## Blueprint
1. Customer traffic hits your e-commerce site
2. CloudFront caches static content for speed
3. AWS EKS scales containerized e-commerce microservices based on demand
4. APIGateway manages APIs for real-time inventory checks against store-level data
5. All sales data streams into S3 and Athena is used for supply chain analytics and demand forecasting


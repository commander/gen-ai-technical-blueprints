# Help users find your products using photos as a reference 

## Business challenge
You want to make it easy for your customers to find desired inventory (e.g. clothing) using a photo as a reference. 

## Tech stack
1. Amazon Sagemaker
2. Amazon Rekognition
3. Amazon OpenSearch + k-NN plugin
4. Amazon S3
5. AWS Lambda (Or ECS Fargate)

## Blueprint
1. A customer uploads a reference photo in the app. The photo is stored in Amazon S3.
2. The upload event triggers AWS Lambda function.
3. Use AWS Rekognition to detect and extract visual features and convert to embeddings
4. This embedding is used to query the OpenSearch service with k-NN plugin enabled, which finds the most visually similar product embeddings from the indexed catalog 
5. The service returns the matching products to the customer in seconds.
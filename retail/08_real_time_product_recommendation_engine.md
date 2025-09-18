# Build a real-time product recommendation engine

## Business challenge

You're a digital retailer trying to increase basket size and customer loyalty. Traditional recommendation engines are too simplistic, often failing to understand a customer's true intent or style beyond basic keywords. This leads to generic suggestions, poor discoverability for unique items in your catalog, and frustrated shoppers who abandon their carts, causing you to leave significant revenue on the table.

## Tech stack
1. Amazon Redshift
2. Amazon OpenSearch with k-NN plugin
3. Amazon SageMaker Feature Store
4. Amazon Kinesis DataStream
5. Amazon Managed Services For Apache Flink
4. AWS Lambda.

# Blueprint
1. User clickstream data streams through Amazon Kinesis Datastream
2. The data stream is processed and enriched by Amazon Managed Services for Apache Flink. Which updates user profiles and embeddings in real-time and stores in Redshift or Sagemake feature store
3. As a user browses, a request is sent to a API on AWS Lambda
4. The service queries OpenSearch (with k-NN Plugin enabled) with the user's embedding to find the most relevant or complementary items
5. A personalized list of products is returned and displayed to the user in milliseconds.
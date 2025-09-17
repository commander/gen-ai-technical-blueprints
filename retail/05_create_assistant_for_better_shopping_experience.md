# Create an assistant for a better shopping experience 

## Business challenge
You're a brand whose traditional support channels, like text-based chatbots and FAQs, feel impersonal, can't visually guide customers through complex processes, and might not create a genuine connection with your audience. 

## Tech stack
1. AWS Bedrock or Sagemaker AI
2. AWS S3 (for 3D assets)
3. EKS (for hosting and scaling)
4. AWS Transcribe and Polly (Speech-to-Text & Text-to-Speech APIs)

## Blueprint
1. A customer asks a troubleshooting question in your app (e.g., "How do I replace the water filter in my coffee machine?").
2. The request is sent to AWS Transcribe (voice) or directly as text
3. Use Amazon Bedrock (for foundational model like Claude) or Sagemake AI (for custom models) to understand the query, identify the intent and generate the text response.
4. A microservice running on AWS EKS fetches a corresponding video (for visual aid) from S3. 
5. The app displays the text and plays the short video, visually guiding the customer through the process and resolving their issue quickly.
6. Amazon Polly is used optionally to convert the text response to speech for a more natural voice assisant.
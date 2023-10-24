# cloud-platforms-coding-challenge

Select one of the two coding challenges and submit a proposed solution by creating a pull request to this repository (see further details in the challenge description)

## Challenge 1 - Terraform AWS Lambda and S3 Setup

### Description

You are tasked with setting up a simple AWS infrastructure using Terraform. Your goal is to create an AWS Lambda function that, when triggered, will read a JSON file from an S3 bucket, process its contents, and log the result to CloudWatch.

### Requirements

1. Use Terraform to define the AWS resources.
2. Create an S3 bucket to store the JSON file.
3. Create an AWS Lambda function.
4. Configure an event trigger for the Lambda function. Whenever a new JSON file is uploaded to the S3 bucket, it should trigger the Lambda function.
5. The Lambda function should read the JSON file, process its contents (e.g., calculate the sum of numbers in the JSON), and log the result to CloudWatch.
6. Write appropriate IAM policies and roles for Lambda and S3 to ensure secure access.
7. Provide a README.md file with clear instructions on how to deploy and test the setup.

### Submission

Please follow these steps to submit your solution:

1. Fork this repository.
2. Create a branch with your solution.
3. Push your branch to your forked repository.
4. Create a pull request (PR) from your branch to the main repository where this coding challenge is defined.

In your pull request, make sure to include your Terraform code and the README.md file explaining how to deploy and test your setup. Your PR will be reviewed based on the evaluation criteria mentioned earlier.

This submission process will allow candidates to submit their solutions directly through GitHub or another version control platform.

### Evaluation Criteria

Your solution will be evaluated based on the following criteria:

1. Correctness: Does the setup work as described in the requirements?
2. Terraform Best Practices: Is the Terraform code well-organized and follows best practices?
3. Security: Are IAM policies and roles properly configured for secure access?
4. Documentation: Is the README.md file clear and informative, providing instructions for deployment and testing?
5. Code Quality: Is the code clean, well-commented, and easy to understand?

## Challenge 2 - Local Kubernetes Deployment with Minio, NATS, and Fission-Deployed Serverless Function

### Description

You are tasked with setting up a local Kubernetes (K8s) deployment with Minio as the storage solution, NATS as a messaging system, and a serverless function using Fission. Minio should send a notification to NATS when an object is stored or updated, and NATS should trigger the Fission-deployed serverless function in response.

### Requirements

1. Use a local Kubernetes cluster (e.g., Minikube or Kind) to define the deployment.
2. Create a Minio instance running within the local cluster. [Minio Documentation](https://docs.min.io/)
3. Set up a NATS server within the local cluster. [NATS Documentation](https://nats.io/documentation/)
4. Configure Minio to send a notification to NATS when an object is stored or updated in a specific Minio folder. [Minio Event Notification Docs](https://docs.min.io/docs/minio-bucket-notification-guide.html)
5. Set up a serverless function using Fission (a FaaS platform) that is triggered by messages received from NATS. [Fission Documentation](https://fission.io/docs/)

### Submission

Please follow these steps to submit your solution:

1. Create a GitHub repository or use an existing one.
2. Write K8s manifests and Helm charts for Minio, NATS, and the Fission function.
3. Provide a README.md file with clear instructions on how to deploy and test the setup in a local cluster. Include links to relevant documentation for reference.
4. Include any additional scripts or files necessary for deployment.

### Evaluation Criteria

Your solution will be evaluated based on the following criteria:

1. Correctness: Does the setup work as described in the requirements?
2. Kubernetes Best Practices: Are K8s resources well-defined and follow best practices?
3. Integration: Does Minio send notifications to NATS when objects are stored or updated, and does the Fission-deployed serverless function respond to these notifications correctly?
4. Documentation: Is the README.md file clear and informative, providing instructions for deployment and testing? Does it include links to relevant documentation?
5. Code Quality: Is the code and configuration clean, well-commented, and easy to understand?

This challenge allows candidates to demonstrate their skills in local Kubernetes setup, Minio, NATS, and Fission for serverless function integration, with easy access to relevant documentation.

# S3 Bucket CloudFormation Stack

This repository contains a CloudFormation template that deploys an S3 bucket with user-selectable encryption types (SSE-S3 and KMS). The template allows the user to input all the necessary values, such as the bucket name and encryption type.

## Deployment Steps

Follow these steps to deploy the CloudFormation stack:

1. **Clone the Repository**: Start by cloning this repository to your local machine.

2. **Navigate to the Template**: Go to the repository's root directory and locate the `s3-bucket-stack.yaml` file.

3. **Customize Parameters**: Open the `s3-bucket-stack.yaml` file and customize the following parameters as needed:
   - `BucketName`: Enter a unique name for the S3 bucket.
   - `EncryptionType`: Select the encryption type for the S3 bucket (`SSE-S3` or `KMS`).

4. **Create the Stack**: Once you've customized the parameters, you can deploy the CloudFormation stack. There are several ways to create the stack, such as using the AWS Management Console, AWS CLI, or AWS SDKs. Here's an example using the AWS Management Console:
   - Open the AWS CloudFormation console.
   - Click on "Create stack" and select "With new resources (standard)".
   - Choose "Upload a template file" and select the `s3-bucket-stack.yaml` file.
   - Click "Next" and provide a unique name for the stack.
   - Fill in the required parameters (`BucketName` and `EncryptionType`) with your desired values.
   - Review and configure any additional settings if necessary.
   - Click "Next" and review the stack details.
   - Finally, click "Create stack" to deploy the S3 bucket.

5. **Monitor Stack Creation**: Wait for the stack creation to complete. You can monitor the progress in the AWS CloudFormation console.

6. **View Stack Outputs**: Once the stack creation is complete, you can retrieve important information about the deployed stack, such as the bucket name and encryption type:
   - Go to the AWS CloudFormation console.
   - Select the deployed stack.
   - Click on the "Outputs" tab to view the stack outputs.

## Outcome

After successfully deploying the CloudFormation stack, you will have an S3 bucket with the desired encryption type. Here's an example of the expected outcome:

![Screenshot from 2023-06-29 18-45-51](https://github.com/eniolastyle/cloudformation-s3/assets/58726365/7fc99b55-5ed9-4c12-b59b-f28b30d401bc)
![Screenshot from 2023-06-29 18-45-59](https://github.com/eniolastyle/cloudformation-s3/assets/58726365/c4915147-ec95-4c9e-804d-11f1e0c10cd5)
![Screenshot from 2023-06-29 18-46-12](https://github.com/eniolastyle/cloudformation-s3/assets/58726365/e6181f7a-2463-498b-a27c-8725e383646b)


## License

This project is licensed under the [MIT License](LICENSE).

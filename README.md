# AWS_Resources_functions_Arrays and Error Handling in Shell Scripting

> This project aims to provide hands-on experience in scripting and automating AWS resource creation while exploring key programming concepts such as functions and arrays.

The included images guide the user through key steps and demonstrate the simulated outputs, making the process easier to follow.

## Step 1: Create a Key Pair

- The first step is to create a key pair and save it to our local PC.

![Keypair](./img/1.%20Keypair.png)

## Step 2: Create a Shell Script

- We will be creating a shell script named `aws_resources.sh`.
- Into the new script, we will add an EC2 creation function.

![EC2](./img/2.%20EC2%20B.png)

- We will also add the S3 creation function to the same script.

![S3](./img/3.%20S3%20B.png)

- After this, we will grant execution permission to the script using the command `chmod +x aws_resources.sh` and execute the script using the command `./aws_resources.sh`.

- In the image below, we can see the output of the script.

![Result](./img/4.%20result.png)

- From the result, EC2 instances have been created successfully.

![EC2](./img/5,%20EC2%20CREARED%20B.png)

- Result from S3 creation:

From the output above, only the EC2 instance was created. The S3 bucket was not created due to an error.

## Error Handling in Shell Scripting

> In the context of our script to create S3 buckets, an error scenario could arise if the bucket already exists when attempting to create it.

> To handle this error, we modified the script to check if the bucket already exists before attempting to create it.

- After updating the script, we confirmed that the profile was set on our terminal and added it to the updated script.

- We also added debug lines in the script to ensure the profile is active.

![Debug](./img/9.%20debug%201.png)

- Updated script:

![Updated Script](./img/8b.%20upsated%20s3%20script.png)
- Result:

![Debug Result](./img/10.%20debug%202.png)

- After executing the script, an S3 bucket was successfully created on our AWS console, as seen below:

![Success](./img/11.%20success.png)

## Summary

This project demonstrates the automation of AWS resource creation using shell scripting. It includes two main functions: one for provisioning EC2 instances and another for creating S3 buckets. The EC2 creation function uses the AWS CLI `run-instances` command to simulate the creation of instances with specific parameters such as AMI ID, instance type, count, and region. The S3 bucket creation function incorporates error handling by checking if a bucket already exists before attempting to create it. Debugging lines were added to ensure the correct AWS profile was active during execution. This project provides a practical approach to learning AWS CLI commands, scripting, and error handling while simulating resource creation in a cost-free environment.

## Error Handling: 
The project demonstrates how to handle errors in shell scripting, such as checking for existing resources before attempting to create them.
Automation: Automating AWS resource creation reduces manual effort and ensures consistency.
Learning Opportunity: This project provides hands-on experience in resource automation, script debugging, and understanding AWS CLI commands.
Through this simulation, the project offers a cost-free learning approach by running locally, making it an excellent resource for beginners and professionals alike.
# AWS_Resources_functions_Arrays

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

![S3](./img/7.%20output.png)

# Summary

This project focuses on automating the creation of AWS resources using shell scripting while incorporating key programming concepts like functions and arrays. It consists of two main functions: one for provisioning EC2 instances and another for setting up S3 buckets. The EC2 provisioning function uses the AWS CLI `run-instances` command to simulate the creation of instances with specific parameters such as AMI ID, instance type, count, and region, ensuring efficiency and scalability. The S3 bucket setup function leverages arrays to loop through a collection of department names, dynamically creating unique bucket names for Marketing, Sales, HR, Operations, and Media. Through this simulation, the project provides hands-on experience in resource automation, script debugging, and understanding AWS CLI commands—all while offering a cost-free learning approach by running locally.
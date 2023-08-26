<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>

# About

This project was made to see my understanding of how to successfully deploy an application on Elastic Beanstalk by manually installing a Jenkins server on an AWS EC2 instance, running a successful pipeline, and achieving a successful deployment on AWS Elastic Beanstalk. Below are the steps I took to achieve that.

## Github:

- **Download zipped files from a repository**
- **Unzip the files from the repository into our local machine**
- **Upload the files into our own Repository**
- **Created a credential key to add to Jenkins later on**

## AWS EC2:

- **Carefully install Jenkins in an EC2 instance**
- **Download and install the correct Python version into our instance**

## Jenkins:

- **Log into Jenkins using the public key from my EC2 instance**
- **Created a pipeline to test out the application files**
- **Added the GitHub credential key to the pipeline**
- **Application files ran successfully after troubleshooting**

## Local Terminal:

- **Jenkins had created a zipped file after successfully running the pipeline due to coding in our application**
- **I had to figure out how to extract the zipped file from Jenkins**
- **Used an SCP command in my local terminal to extract the zipped file from Jenkins**

## AWS Elastic Beanstalk:

- **I had to create IAM roles for my Elastic Beanstalk and EC2**
- **Added the application name "URL-shortener"**
- **Uploaded the zipped application file I extracted from Jenkins**
- **Added a VPC and availability zones to the application**
- **Application ran successfully**

## Troubleshooting:

During this project, I encountered some difficulties while attempting to build a pipeline. When I attempted to run it the first time, it would stop and ask me to continue, resulting in a failure regardless. After troubleshooting, I found out it was a network issue on my end. After fixing the problem, I ran the pipeline again, and it was successful. Another problem I encountered was the extraction of the zipped file. During my SCP commands, I was failing to notice a syntax error on my end.
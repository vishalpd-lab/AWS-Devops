# AWS-Devops
Aws Zero to Hero
Day 1: Task
Create EC2 instance, create IAM user, Create S3 bucker, one user who sit other location and accecc from their laptop assign IAM role for that user and also he see s3 bucket/data object

Step 1. Create EC2 instance
choose US west 2 availability zone 

Launch instance > select Ubuntu > t3 micro > key pair > 
<img width="1090" height="886" alt="image" src="https://github.com/user-attachments/assets/d5342493-63c3-4ecc-97a7-d9c3e626fff3" />

 
Create New security group > Allow SSH traffic > select memory as per requirement > Launch EC2

 
Instance is Ready:

 




Step 2: Create IAM user with policies
   We have created test1 user and assign ec2 and s3 access for this user 

  
Click and Create user 

 
  Step 2: create S3 bucket > 

 
Step 4: Uplode something data into our created S3 bucket 

 
Step 5: Now we have from outside from aws, access this created S3 bucket.
For that we configure AWS cli 

Create Access Key :
IAM > user > Security credentials > Access Key > create Access key > choose Command line CLI

 
 
                                                                                                                                                 
 








Step 6 : Now connect EC2 instance for access aws cli >

 
Step 7 : Install aws cli v2 on this instance >
  # sudo apti install unzip 

To install the AWS CLI, run the following commands.
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
 
Now configure aws credentials :

#aws configure          ---- give aws access and secreat key from IAM user


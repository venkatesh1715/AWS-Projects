# CloudFormation S3 Template
```
## Problem Statement:
You work for XYZ Corporation. Your team is asked to deploy similar architecture multiple times for testing, development, and production purposes. Implement CloudFormation for the tasks assigned to you below.

## Tasks To Be Performed:
1) Create a template which can create an S3 bucket named “Intellipaat-<yourname >”
2) The template should be able to enable versioning for the bucket created.
```

# CloudFormation VPC Template
```
## Problem Statement:
You work for XYZ Corporation. Your team is asked to deploy similar architecture multiple times for testing, development, and production purposes. Implement CloudFormation for the tasks assigned to you below.

## Tasks To Be Performed:
1) Create a template with 1 VPC and 1 public subnet.
2) Launch an Amazon Linux EC2 instance in the public subnet and tag the instance as “CFinstance”
```
# SQS-And-SES-Assignment

Problem Statement:
You work for XYZ Corporation. Your team is asked to deploy similar architecture multiple times for testing, development, and production purposes. Implement CloudFormation for the tasks assigned to you below.
```
Tasks To Be Performed:
1) Create a FIFO SQS queue and test by sending messages.
2) Register your mail in SES and send a test mail to yourself.
```
# CloudFormation-SNS-Assignment

Problem Statement:
You work for XYZ Corporation. Your team is asked to deploy similar architecture multiple times for testing, development, and production purposes. Implement CloudFormation for the tasks assigned to you below.
```
Tasks To Be Performed:
1) Use the template from CloudFormation task 1.
2) Add Notification to the CloudFormation stack using SNS so that you get a notification via mail for every step of the stack creation process.
```
# Case-Study-–- `Multi-Tier-Architecture`
```
Problem Statement:
You work for XYZ Corporation. Your corporation wants to launch a new web-based application. The development team has prepared the code but it is not tested yet. The development team needs the system admins to build a web server to test the code but the system admins are not available.

Tasks To Be Performed:
1) Web tier: Launch an instance in a public subnet and that instance should allow HTTP and SSH from the internet.
2) Application tier: Launch an instance in a private subnet of the web tier and it should allow only SSH from the public subnet of Web Tier-3.
3) DB tier: Launch an RDS MYSQL instance in a private subnet and it should allow connection on port 3306 only from the private subnet of Application Tier-4.
4) Setup a Route 53 hosted zone and direct traffic to the EC2 instance.

You have been also asked to propose a solution so that:
1) Development team can test their code without having to involve the system admins and can invest their time in testing the code rather than provisioning, configuring and updating the resources needed to test the code.
2) Make sure when the development team deletes the stack, RDS DB instances should not be deleted.
```
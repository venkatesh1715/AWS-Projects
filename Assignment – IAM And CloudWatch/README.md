# IAM Users Assignmen --1
```
## Problem Statement:
You work for XYZ Corporation. To maintain the security of the AWS account and the resources you have been asked to implement a solution that can help easily recognize and monitor the different users.

## Tasks To Be Performed:
1) Create 4 IAM users named “Dev1”, “Dev2”, “Test1”, and “Test2”.
2) Create 2 groups named “Dev Team” and “Ops Team”.
3) Add Dev1 and Dev2 to the Dev Team.
4) Add Dev1, Test1 and Test2 to the Ops Team.
```

# IAM Policies Assignment --2
```
## Problem Statement:
You work for XYZ Corporation. To maintain the security of the AWS account and the resources you have been asked to implement a solution that can help easily recognize and monitor the different users.

## Tasks To Be Performed:
1) Create policy number 1 which lets the users to:
	a. Access S3 completely
	b. Only create EC2 instances
	c. Full access to RDS
2) Create a policy number 2 which allows the users to:
	a. Access CloudWatch and billing completely
	b. Can only list EC2 and S3 resources.
3) Attach policy number 1 to the Dev Team from task 1
4) Attach policy number 2 to Ops Team from task 1.
```

# IAM Roles Assignment –-3
```
## Problem Statement:
You work for XYZ Corporation. To maintain the security of the AWS account and the resources you have been asked to implement a solution that can help easily recognize and monitor the different users.

## Tasks To Be Performed:
1) Create a role which only lets user1 and user2 from task 1 to have complete access to VPCs and DynamoDB.
2) Login into user1 and shift to the role to test out the feature.
```

# CloudWatch Dashboard Assignment –-4
```
## Problem Statement:
You work for XYZ Corporation. To maintain the security of the AWS account and the resources you have been asked to implement a solution that can help easily recognize and monitor the different users. Also, you will be monitoring the machines created by these users for any errors or misconfigurations.

## Tasks To Be Performed:
1) Create a dashboard which lets you check the CPU utilization and networking for a particular EC2 instance.
```

# CloudWatch Alarms Assignment –-5
```
## Problem Statement:
You work for XYZ Corporation. To maintain the security of the AWS account and the resources you have been asked to implement a solution that can help easily recognize and monitor the different users. Also, you will be monitoring the machines created by these users for any errors or misconfigurations.

## Tasks To Be Performed:
1) Create a CloudWatch billing alarm which goes off when the estimated charges go above $500.
2) Create a CloudWatch alarm which goes off to an Alarm state when the CPU utilization of an EC2 instance goes above 65%. Also add an SNS topic so that it notifies the person when the threshold is crossed.
```
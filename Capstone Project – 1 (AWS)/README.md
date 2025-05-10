# 🚀 Building a Resilient Multi-Tier Architecture on AWS EC2 with Auto Scaling and RDS

## 📘 Overview

This project demonstrates the deployment of a highly available, scalable, and secure multi-tier web application architecture on Amazon Web Services (AWS). The architecture leverages key AWS services such as Amazon EC2, Auto Scaling Groups, and Amazon RDS to ensure optimal performance and resilience.

## 🎯 Objectives

* **High Availability**: Distribute resources across multiple Availability Zones to prevent single points of failure.
* **Scalability**: Implement Auto Scaling to handle varying traffic loads efficiently.
* **Security**: Configure security groups and network ACLs to protect resources.
* **Cost Optimization**: Utilize AWS Free Tier eligible services where possible.

## 🧱 Architecture Components

* **Web Tier**: Amazon EC2 instances behind an Application Load Balancer (ALB) to serve the PHP-based website.
* **Application Tier**: Scalable EC2 instances managed by an Auto Scaling Group to handle business logic.
* **Database Tier**: Amazon RDS (MySQL) instance for persistent data storage.

## 🛠️ Implementation Steps

1. **Launch EC2 Instances**:

   * Deploy EC2 instances in multiple Availability Zones.
   * Install and configure Apache and PHP to serve the web application.

2. **Configure Auto Scaling**:

   * Create a Launch Template with the necessary configurations.
   * Set up an Auto Scaling Group with a minimum of 2 instances and desired scaling policies.

3. **Set Up Amazon RDS**:

   * Launch a MySQL RDS instance with the following configurations:

     * **Database Name**: `intel`
     * **Table Name**: `data`
     * **Master Username**: `admin`
     * **Master Password**: `intel123`

4. **Update Application Configuration**:

   * Modify the web application's database connection settings to point to the RDS endpoint.

5. **Configure Security Groups**:

   * Allow HTTP (port 80) and SSH (port 22) traffic to EC2 instances.
   * Permit MySQL/Aurora (port 3306) traffic from EC2 instances to the RDS instance.

6. **Testing and Validation**:

   * Access the web application via the ALB DNS name.
   * Verify data persistence by interacting with the application and checking the RDS database.

## 📁 Repository Structure

```
Capstone Project – 1 (AWS)/
├── Application/
│   └── index.php
│   └── images
├── Deploying a Multi-Tier Website Using AWS EC2.pdf
└── README.md
```

## 🧠 Learnings and Insights

* Gained hands-on experience with AWS EC2, Auto Scaling, and RDS services.
* Understood the importance of designing for failure and implementing redundancy.
* Learned to configure security groups and manage network traffic effectively.
* Recognized the value of infrastructure as code for repeatable deployments.

## 📚 References

* [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
* [AWS Auto Scaling Documentation](https://docs.aws.amazon.com/autoscaling/)
* [AWS RDS Documentation](https://docs.aws.amazon.com/rds/)

# 🚀 High Availability Website Deployment Using AWS Elastic Beanstalk and RDS

## 📘 Overview

This project demonstrates the deployment of a highly available, scalable, and secure PHP web application using AWS Elastic Beanstalk and Amazon RDS. By decoupling the database from the application environment, we achieve greater flexibility, easier maintenance, and enhanced scalability.

## 🎯 Objectives

* **High Availability**: Ensure the application remains accessible and operational across multiple Availability Zones.
* **Scalability**: Implement Auto Scaling to handle varying traffic loads efficiently.
* **Security**: Configure security groups and network ACLs to protect resources.
* **Decoupled Architecture**: Separate the database from the application lifecycle for better manageability.

## 🧱 Architecture Components

* **Application Tier**: PHP application deployed on AWS Elastic Beanstalk.
* **Database Tier**: Amazon RDS (MySQL) instance hosted externally to the Elastic Beanstalk environment.
* **Networking**: Properly configured security groups to allow secure communication between the application and database tiers.

## 🛠️ Implementation Steps

1. **Launch Amazon RDS Instance**:

   * Deploy a MySQL RDS instance with the following configurations:

     * **Database Name**: `intel`
     * **Master Username**: `admin`
     * **Master Password**: `intel123`
   * Ensure the RDS instance is in a Multi-AZ deployment for high availability.
   * Configure the RDS security group to allow inbound traffic on port 3306 from the Elastic Beanstalk environment's security group.

2. **Create Elastic Beanstalk Environment**:

   * Initialize a new PHP environment in Elastic Beanstalk.
   * Configure environment variables to store database connection details (e.g., host, username, password).
   * Deploy the PHP application code to the environment.

3. **Configure Security Groups**:

   * Modify the Elastic Beanstalk environment's security group to allow outbound traffic to the RDS instance.
   * Ensure the RDS security group allows inbound traffic from the Elastic Beanstalk security group on the appropriate port.

4. **Implement Auto Scaling**:

   * Set up Auto Scaling policies within Elastic Beanstalk to handle traffic fluctuations.
   * Define minimum and maximum instance counts based on anticipated load.

5. **Testing and Validation**:

   * Access the application via the provided Elastic Beanstalk URL.
   * Perform CRUD operations to ensure proper communication between the application and the RDS database.

## 📁 Repository Structure

```
Capstone Project – 2 (AWS)/
├── Website Orchestration.pdf
└── README.md
```

## 🧠 Learnings and Insights

* Gained hands-on experience with AWS Elastic Beanstalk and Amazon RDS.
* Understood the importance of decoupling application and database tiers for better scalability and manageability.
* Learned to configure security groups to ensure secure communication between AWS resources.
* Implemented Auto Scaling to handle varying traffic loads efficiently.

## 📚 References

* [Deploying a high-availability PHP application with an external Amazon RDS database to Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/php-ha-tutorial.html)
* [AWS Elastic Beanstalk Documentation](https://docs.aws.amazon.com/elasticbeanstalk/)
* [Amazon RDS Documentation](https://docs.aws.amazon.com/rds/)

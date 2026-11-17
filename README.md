# aws-ec2-web-server-management
Hands on AWS project exploring EC2 provisioning, web server deployment, monitoring and infrastructure management
 # AWS EC2: Launching, Managing and Monitoring a Web Server

## Project Overview

This is a hands-on AWS project focused on launching, configuring and managing an Amazon EC2 instance.

The project explores how to deploy a simple Apache web server, configure network access, monitor instance health and understand infrastructure scaling.

## Tools and Technologies

- Amazon Web Services (AWS)
- Amazon EC2
- Amazon Linux 2023
- Apache HTTP Server
- Amazon EBS
- Amazon CloudWatch
- Security Groups

## Project Objectives

1. Launch an Amazon EC2 instance.
2. Deploy a web server using User Data.
3. Monitor EC2 instance health.
4. Configure Security Groups to allow HTTP traffic.
5. Resize compute and storage resources.
6. Understand termination protection.

## Step 1: Launch an EC2 Instance

I accessed the AWS Management Console and navigated to EC2.

I explored the instance launch configuration, including:

- Amazon Machine Image (AMI)
- Instance type
- Network settings
- Security Groups
- Storage configuration

## Step 2: Deploy a Web Server Using User Data

I used the following commands to automate Apache web server installation.

```bash
#!/bin/bash
yum -y install httpd
systemctl enable httpd
systemctl start httpd
echo '<html><h1>Hello From Your Web Server!</h1></html>' > /var/www/html/index.html
```

## Step 3: Monitor the EC2 Instance

Explored instance status checks and CloudWatch monitoring to understand how AWS monitors infrastructure health and performance.

## Step 4: Configure HTTP Access

Configured the Security Group to permit HTTP traffic through port 80.

## Step 5: Resize the Instance

Practised changing the instance type from t3.micro to t3.small.

Also explored increasing the EBS volume from 8 GiB to 10 GiB.

## Step 6: Test Termination Protection

Explored how termination protection prevents accidental deletion of an EC2 instance.

## Key Learnings

- EC2 provisioning and configuration.
- Automated web server deployment.
- Linux-based server management.
- Security Group configuration.
- HTTP networking.
- Cloud monitoring.
- Infrastructure scaling.
- Resource protection.

## Conclusion

This practical exercise strengthened my understanding of AWS EC2 and the fundamentals of cloud infrastructure management.

I am documenting my hands-on learning experiences as I continue developing my Cloud and DevOps engineering skills.


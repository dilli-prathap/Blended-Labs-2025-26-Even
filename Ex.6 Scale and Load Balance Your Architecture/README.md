# Lab 6 – Scale and Load Balance Your Architecture

## Title

## Scale and Load Balance Your Architecture
Author : DILLI PRATHAP   
Reg no : 212224110014
Date : 19-03-2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

## **Workflow (Short Version)**

1. Logged into AWS and reviewed existing EC2 setup.
2. Created a launch template with AMI, instance type, and user data.
3. Created an Auto Scaling Group with min, max, and desired capacity.
4. Configured an Application Load Balancer and target group.
5. Attached the Auto Scaling Group to the load balancer.
6. Set scaling policies based on CPU utilization using CloudWatch.
7. Tested by generating traffic and verified automatic scaling and load distribution.

---

## Output Screenshots 
<img width="1222" height="929" alt="Screenshot 2026-03-19 185929" src="https://github.com/user-attachments/assets/24a7a259-43e0-4e0c-b46a-81abc22c7203" />
<img width="1215" height="925" alt="Screenshot 2026-03-19 190309" src="https://github.com/user-attachments/assets/f87df6ec-823e-4261-9bbd-71f5933d0cb0" />
<img width="1225" height="952" alt="Screenshot 2026-03-19 190629" src="https://github.com/user-attachments/assets/a6565817-bf5d-418c-b67f-e1802dc2062a" />
<img width="1220" height="981" alt="Screenshot 2026-03-19 193334" src="https://github.com/user-attachments/assets/831e5e17-7b58-4cfe-92a6-c8b67d0b34d8" />
<img width="1487" height="540" alt="Screenshot 2026-03-19 193832" src="https://github.com/user-attachments/assets/b93abf90-b996-4dfe-9abe-2f7688d39ddb" />
<img width="1213" height="962" alt="Screenshot 2026-03-19 202829" src="https://github.com/user-attachments/assets/ba09d10f-d02d-4e15-9a5b-a6bbabd782d2" />


---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.

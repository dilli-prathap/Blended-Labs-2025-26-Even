# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: DILLI PRATHAP 
* **Register Number**: 212224110014
* **Date of Submission**: 27-02-2026
---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

I logged in to the AWS Management Console and opened Amazon Elastic Compute Cloud (EC2).

I launched a new EC2 instance using Amazon Linux 2 AMI and selected the t2.micro under the free tier.

I created a new key pair to securely connect to the instance and downloaded the .pem file.

I configured a security group allowing SSH (Port 22) from my IP address and HTTP (Port 80) from anywhere (0.0.0.0/0).

After launching the instance, I connected to it using SSH with the key pair and accessed the Linux terminal.

I performed basic instance operations such as stop, start, and reboot from the EC2 console and observed the instance state changes.

I monitored the instance performance using CPU utilization, network traffic, and status checks in the Monitoring tab (via Amazon CloudWatch).

Finally, I terminated the EC2 instance after completing the lab to avoid unnecessary AWS charges.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1160" height="1016" alt="Screenshot 2026-02-26 161514" src="https://github.com/user-attachments/assets/78e7ce80-d9e9-4f94-9574-e2ccf7785c92" />

---

### Screenshot 2: SSH Connection to Instance

<img width="1257" height="460" alt="Screenshot 2026-02-27 093353" src="https://github.com/user-attachments/assets/7a37b241-eac8-42c7-b4a6-9ee140769241" />

---

### Screenshot 3: Instance Monitoring / Status
## t2-micro:

<img width="1668" height="356" alt="Screenshot 2026-02-27 082616" src="https://github.com/user-attachments/assets/79378b0c-a62f-4dd1-8d9e-b91ffe13e435" />

## t2-small:
<img width="1445" height="970" alt="Screenshot 2026-02-27 092158" src="https://github.com/user-attachments/assets/3a8ca9e0-2f92-49df-8d2d-0be8f0356ef6" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

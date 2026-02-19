# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: DILLI PRATHAP D
* **Register Number**: 212224110014
* **Date of Submission**: 19-02-2026
---

## Objective

The objective of this experiment is to understand how to design and configure a basic network infrastructure in AWS using a Virtual Private Cloud (VPC). This lab focuses on creating a VPC with a public subnet, configuring an Internet Gateway and route table, launching an EC2 instance, and hosting a simple web server that can be accessed over the internet.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity

---

## Tools Used

* AWS Management Console
* Amazon VPC
* Amazon EC2
* Internet Gateway
* Route Table
* Security Groups

---

## Tasks Performed

### Task 1: Create a VPC

Create a new Virtual Private Cloud (VPC) with a private IP address range. The VPC acts as a logically isolated network in AWS where all other resources will be deployed.

Students should create a VPC with an appropriate CIDR block (for example, 10.0.0.0/16) and assign a meaningful name.


### Task 2: Create a Public Subnet

Create a subnet inside the VPC to host public resources. Enable auto-assign public IPv4 so that instances launched in this subnet receive a public IP address.

The subnet should use a smaller CIDR range (for example, 10.0.1.0/24).


### Task 3: Create and Attach Internet Gateway

Create an Internet Gateway (IGW) and attach it to the VPC. This allows communication between resources in the VPC and the internet.


### Task 4: Configure Route Table

Create a route table and add a default route (0.0.0.0/0) pointing to the Internet Gateway. Associate this route table with the public subnet.

This step ensures that traffic from the subnet can reach the internet.


### Task 5: Create Security Group

Create a security group to act as a virtual firewall for the EC2 instance. Configure inbound rules to allow:

SSH on port 22

HTTP on port 80


### Task 6: Launch EC2 Instance

Launch an EC2 instance inside the public subnet using Amazon Linux 2 AMI and a suitable instance type (t2.micro).

Attach the previously created security group and key pair.


### Task 7: Configure Web Server

Install and start a web server (Apache HTTPD) on the EC2 instance using user data or manual commands.

Create a simple HTML page and verify that it can be accessed from a web browser using the public IP address of the instance.---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. I created a VPC in Amazon Web Services with the CIDR block 10.0.0.0/16 to set up a private network.
2. I created a public subnet (10.0.1.0/24) and enabled auto-assign public IP.
3. I attached an Internet Gateway and configured a route table to allow internet access.
4. I created a security group allowing SSH (22) and HTTP (80).
5. I launched an EC2 instance, installed Apache, and verified the website using the public IP.

## Output Screenshots (Attach 3)

### Screenshot 1: VPC and Subnet Details

<img width="1081" height="938" alt="Screenshot 2026-02-19 112026" src="https://github.com/user-attachments/assets/f1da883c-f49a-4520-b52b-294188f60122" />

---

### Screenshot 2: EC2 Instance Running

<img width="1483" height="445" alt="Screenshot 2026-02-19 115155" src="https://github.com/user-attachments/assets/06f597bc-9b79-4a1e-9b84-bcaba4ceae12" />


---

### Screenshot 3: Web Server Output in Browser

<img width="1458" height="449" alt="Screenshot 2026-02-19 115045" src="https://github.com/user-attachments/assets/0c0e6488-e42d-457d-acbf-ec10bdb5e072" />


---

## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.

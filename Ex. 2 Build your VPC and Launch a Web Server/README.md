# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: GURUPARAN G
* **Register Number**: 212224220030
* **Date of Submission**: 15.02.26

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

1.  A Virtual Private Cloud (VPC) was designed and created with the CIDR block 10.0.0.0/16 to establish a secure and isolated network
environment within AWS.
2. A public subnet was configured within the VPC with the CIDR range 10.0.1.0/24, and auto-assign public IPv4 addresses was
enabled to allow internet connectivity for instances.
3. An Internet Gateway was created and attached to the VPC, followed by the setup of a route table with a default route (0.0.0.0/0)
pointing to the gateway, and the route table was associated with the public subnet.
4. A security group was established to permit inbound SSH (port 22) and HTTP (port 80) traffic, and an EC2 instance was launched
using the Amazon Linux 2 AMI, associated with the security group and a key pair.
5. The Apache HTTPD web server was installed and started on the EC2 instance, a simple HTML webpage was created, and its
accessibility was verified through the public IP address of the instance via a web browser.

---

## Output Screenshots (Attach 3)

### Screenshot 1: VPC and Subnet Details

<img width="1185" height="617" alt="image" src="https://github.com/user-attachments/assets/e704bd89-ae6c-49b2-afae-2d94aa066b6a" />


---

### Screenshot 2: EC2 Instance Running

<img width="1192" height="628" alt="image" src="https://github.com/user-attachments/assets/2d78d86d-833e-4bd3-b6c5-924b8b25e1d3" />

<img width="1191" height="631" alt="image" src="https://github.com/user-attachments/assets/71bae6c4-03e2-4d41-b06f-f39500efee3b" />

---

### Screenshot 3: Web Server Output in Browser


<img width="882" height="316" alt="image" src="https://github.com/user-attachments/assets/83ac6b9f-ce9d-4283-b406-1f5e9101c33c" />

---

## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.

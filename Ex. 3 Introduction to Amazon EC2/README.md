# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: GURUPARAN G
* **Register Number**:212224220030
* **Date of Submission**: 17/03/2026

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

1.Logged into the AWS Management Console and opened the EC2 dashboard to review the available sections like Instances, AMIs, Key Pairs, Security Groups, and Elastic IPs. This helped me understand how EC2 resources are organized.

2.Launched a new virtual machine by selecting Amazon Linux 2 AMI and choosing the t2.micro instance type under the free tier. Configured basic settings including instance name, key pair, and default network options.

3.Created and configured a Security Group to control inbound traffic. Allowed SSH (port 22) access from my IP for secure remote login and HTTP (port 80) access from anywhere to enable web traffic.

4.Connected to the running EC2 instance using SSH with the downloaded key pair. Verified successful connection by accessing the command line of the Amazon Linux instance.

5.Performed basic instance management operations such as Stop, Start, and Reboot from the EC2 console, observing the corresponding state changes and understanding instance lifecycle behavior.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1897" height="1020" alt="image" src="https://github.com/user-attachments/assets/f4f8d23c-a42a-423a-8d2c-55b41e0ba7e7" />

<img width="1910" height="1063" alt="image" src="https://github.com/user-attachments/assets/0c32c63c-762d-4088-9730-e02240cc3d4e" />


---

### Screenshot 2: SSH Connection to Instance

<img width="1903" height="1018" alt="image" src="https://github.com/user-attachments/assets/6c478f75-e63c-48ef-9df7-ff99ca0d969e" />


---

### Screenshot 3: Instance Monitoring / Status

<img width="1905" height="1053" alt="image" src="https://github.com/user-attachments/assets/a8ec4df9-939c-4063-a219-1cf772147058" />


---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

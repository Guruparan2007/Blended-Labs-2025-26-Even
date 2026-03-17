# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: GURUPARAN G
* **Register Number**: 212224220030
* **Date of Submission**: 17/03/2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1.Launched an EC2 instance with Amazon Linux 2 and configured key pair and security group.
2.Enabled SSH (Port 22) and database port (3306/5432) in the security group.
3.Connected to the EC2 instance using SSH.
4.Installed and started the database server, then configured root password.
5.Created a sample database, added a table, inserted records, and tested with SQL queries.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

(<img width="1915" height="1195" alt="image" src="https://github.com/user-attachments/assets/fbaa387b-0127-476b-bf90-eb40bd4b021d" />


---

### Screenshot 2: Database Service Running

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/6e2e5b35-3f9e-4546-809c-5c1bfc059bac" />




---

### Screenshot 3: Sample Database and Table

<img width="1918" height="1195" alt="image" src="https://github.com/user-attachments/assets/359b67b5-31ba-42c2-922c-12717cc22aeb" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst

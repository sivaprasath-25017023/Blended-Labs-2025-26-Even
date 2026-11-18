# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: SIVAPRASATH R
* **Register Number**: 212224243007
* **Date of Submission**: 18/11/26

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

(Write the steps you followed in your own words)

1.The EC2 Dashboard was accessed through the AWS Management Console to explore the Amazon EBS volume types.

2.A new EBS volume was created by selecting the volume type, size, and the same Availability Zone as the EC2 instance.

3.The created EBS volume was attached to the running EC2 instance as an additional block device.

4.The attached volume was formatted using the ext4 file system and mounted to a directory in the EC2 instance.

5.Sample data was stored in the mounted volume, and after rebooting the instance, data persistence was verified successfully.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1919" height="1199" alt="Screenshot 2026-10-28 134443" src="https://github.com/user-attachments/assets/325d609a-fb4c-4312-97dc-1db70a792262" />



---


<img width="1919" height="1199" alt="Screenshot 2026-10-28 135147" src="https://github.com/user-attachments/assets/ba4d30d2-cee5-42a1-952c-aa75a906ce31" />

<img width="1919" height="1199" alt="Screenshot 2026-10-28 135924" src="https://github.com/user-attachments/assets/9134923a-a641-4396-a7ed-e131f7e4ba02" />
<img width="1919" height="1199" alt="Screenshot 2026-10-28 140345" src="https://github.com/user-attachments/assets/207d6f96-079f-4556-9fb8-41aa937d58c8" />


---

### Screenshot 3: Instance Monitoring / Status

<img width="1919" height="1199" alt="Screenshot 2026-10-28 141122" src="https://github.com/user-attachments/assets/2d299608-c472-4dcd-be96-b38c24d23a90" />


<img width="1914" height="1199" alt="Screenshot 2026-10-28 143606" src="https://github.com/user-attachments/assets/2fd46b9a-03e5-4644-92e1-68bfa06ff3e8" />


---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

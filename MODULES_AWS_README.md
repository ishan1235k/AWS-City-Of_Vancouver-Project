#Modules_and_Draw.io_Screenshots 
# MODULE 1 – AWS Cloud Concepts

This document summarizes the design and key concepts covered in Modules of the AWS , focused on cloud computing models, data security, and operational design.

---

## 🌐 Traditional vs Cloud Computing Model

![Traditional vs Cloud Computing](https://github.com/user-attachments/assets/c3bac4e7-5fc0-494b-8b2d-760b454e8a5b)


This diagram compares the traditional computing model with the cloud computing model, highlighting differences in dataset location, access methods, and privacy controls.

---

## ⚙️ Module 1 Design

![Module 1 Design](https://github.com/user-attachments/assets/65e573df-d81c-4bc1-ab81-b3bfd73da991)


This diagram illustrates the overall architectural design for the module, demonstrating data center setup, operational environment, and general server structure.

---

## 🏗️ Module 1 IaaS, PaaS, SaaS Design

![Module 1 IPS design](https://github.com/user-attachments/assets/d865585c-0cc7-4238-82d7-c05eec8c4e33)


This figure presents the IaaS, PaaS, and SaaS layers, showing responsibilities shared between HR, AWS teams, and operations teams.

---

## 🔑 IaaS vs PaaS vs SaaS Privacy and Access

![Module 1 IvPvsS](https://github.com/user-attachments/assets/0df844a1-ac26-4281-8cf5-a557077ae114)


A summary table outlining dataset location, access levels, and privacy responsibilities across the IaaS, PaaS, and SaaS models.

---

## ✅ Module 1 Knowledge Check

![Module 1 KC](https://github.com/user-attachments/assets/c3d392a8-0f00-4490-ae69-b0b12432ba0e)

The knowledge check confirms understanding of Module 1 concepts. Example result: 90/100.

# MODULE 2 – AWS Cost and Pricing Concepts

This section summarizes key case studies, pricing tools, and support plans covered in Module 2.

---

## 💼 Case Study #4 – Total Cost of Ownership & AWS Pricing Calculator

![Module 2 Case studies and Price Calculatos](https://github.com/user-attachments/assets/34b3bdb0-aa4c-4ed5-aa4e-77c746e21349)


This image includes:
- **Case Study #4: Total Cost of Ownership (Delaware North)** – Highlights cost challenges with on-premises infrastructure, and illustrates the TCO benefits after migrating workloads to AWS.
- **Case Study #5: AWS Pricing Calculator** – Displays pricing estimations for AWS services, with detailed monthly and annual cost summaries, and configurations used.
- **Case Study #6: AWS Support Plan** – Shows the selected AWS support plan with justifications aligned to departmental business needs.

---

## ✅ Module 2 Knowledge Check

![Module 2 KC](https://github.com/user-attachments/assets/79de731f-07c8-41db-b7aa-7fede03cdace)

This image displays the submission confirmation and grade for Module 2 Knowledge Check, with a score of 70/100.

# MODULE 3 – AWS Global Infrastructure and Content Delivery

This section summarizes Module 3 concepts focused on AWS global infrastructure, content delivery, and data privacy.

---

## 🌍 AWS Global Infrastructure Design

![Module 3 Global Infrastructure](https://github.com/user-attachments/assets/7a0ecfbe-5ab9-414a-83ce-58eca1c88294)


This diagram illustrates AWS global infrastructure components:
- **Regions**: Example shown is Virginia, with two availability zones (N. Virginia and Oregon).
- **Availability Zones**: Each zone hosts a general virtual server with CPU, memory, NIC, and dataset storage.
- **Edge Locations & Regional Edge Cache**: These components are used to enhance content delivery, speed up repeated access, and reduce latency for students accessing data.

The table summarizes dataset location, access, and privacy:
- **Regional Edge Cache**: Data stored near edge sites, speeds up repeated access, encrypted cache data.
- **Edge Location**: Closest point of presence, low latency delivery, encrypted content delivery.
- **Region**: Data in Virginia, IAM-based access, KMS-managed privacy.

---

## ✅ Module 3 Knowledge Check
![Module 3 KC](https://github.com/user-attachments/assets/b8b34260-8f62-446a-b0e0-644f07b33907)
This image confirms completion of Module 3 Knowledge Check with a score of 80/100.

# MODULE 4 – AWS IAM and Access Management

This section summarizes Module 4 concepts, including responsibility models, IAM practices, and lab work.

---

## 🤝 Case Study #8 – Who is Responsible (UCW vs AWS)

![Module 4 ucw vs aws](https://github.com/user-attachments/assets/0fcb8fcd-fcdb-468b-acf1-b5001e8b3ee9)


This diagram illustrates shared responsibility between UCW and AWS:
- **EC2**: UCW manages the instance; AWS ensures infrastructure uptime.
- **Platform**: UCW handles OS and middleware updates; AWS manages virtualization and hardware.
- **Software**: UCW is responsible for application management.
- **Dataset**: UCW oversees data security and backup; AWS ensures storage durability.
The visual also shows operational team roles linked to these responsibilities.

---

## 🔐 AWS IAM Lab Summary

![Lab 1 IAM](https://github.com/user-attachments/assets/31ff5bae-8fb3-4e52-bc86-a70949629d66)


This image shows the AWS IAM lab task summary:
- Added users to specific IAM groups (S3-Support, EC2-Support, EC2-Admin).
- Tested access policies through login and service access attempts.
- Achieved a score of 30/40, demonstrating successful completion of key objectives.

---

## ✅ Module 4 Knowledge Check

![Module 4 KC](https://github.com/user-attachments/assets/a0d56c7d-beb4-490c-81a3-5c735031e2d8)
This image shows completion of the Module 4 Knowledge Check with a score of 80/100.

# MODULE 5 – AWS Networking and VPC

This section summarizes Module 5, covering AWS Virtual Private Cloud (VPC), networking components, and lab work.

---

## 🌐 Lab 2 – Build Your VPC

![Lab 2 Build Your VPC](https://github.com/user-attachments/assets/aa07b707-3d48-4986-9d9e-d654e5663ebb)


This image shows the lab submission for building a custom VPC:
- **Tasks completed**: VPC creation, subnets setup, route table associations, security group setup, EC2 instance deployment, and website accessibility.
- **Score**: 30/30, reflecting successful configuration and deployment of networking components, ensuring connectivity and security compliance.

---

## ✅ Module 5 Knowledge Check

![Module 5 KC](https://github.com/user-attachments/assets/e439092f-2b23-419a-9ac1-680958454ba7)


This image displays the Module 5 Knowledge Check result:
- **Score**: 80/100 (80%).
- Demonstrates completion and understanding of AWS networking, VPC, and related services.

# MODULE 6 – AWS Lambda and Serverless Concepts

This section summarizes Module 6, covering AWS Lambda, serverless automation, and lab work.

---

## ⚡ Lab 3 – AWS Lambda Function

![Lab 3Lamda Function](https://github.com/user-attachments/assets/9c8870c5-b491-4605-b0da-ef7a611f8baa)


This image shows the lab summary for creating and configuring an AWS Lambda function:
- The Lambda function was triggered by an Amazon EventBridge event to stop an EC2 instance on schedule.
- Tasks included creating the Lambda function, configuring the schedule, setting permissions via IAM, and successfully stopping the EC2 instance.
- **Score**: 20/20, indicating all tasks were correctly completed.

---

## ✅ Module 6 Knowledge Check

![Module 6 KC](https://github.com/user-attachments/assets/fcee4983-69ea-4ccc-ae3f-f6a670323067)


This image shows completion of the Module 6 Knowledge Check:
- **Score**: 70/100 (70%).
- Demonstrates understanding of serverless concepts and AWS Lambda use cases.

# MODULE 7 – AWS Storage: EBS and Snapshots

This section summarizes Module 7, focused on AWS Elastic Block Store (EBS), snapshot management, and lab tasks.

---

## 💾 Lab 4 – Working with EBS

![Lab 4 Working with EBS](https://github.com/user-attachments/assets/87d415f9-2a07-4852-89e1-aca5d8bb9885)


This image shows the lab completion for EBS volume and snapshot management:
- Successfully created and attached an Amazon EBS volume to an EC2 instance.
- Formatted the volume, added files, and created/restored snapshots.
- **Score**: 25/25, indicating full completion of all lab tasks, including volume creation, attachment, mounting, snapshot creation, and restoration.

---

## ✅ Module 7 Knowledge Check

![Module 7 KC](https://github.com/user-attachments/assets/12438919-bb47-4ed8-9db0-3d41a7695638)


This image confirms completion of the Module 7 Knowledge Check:
- **Score**: 90/100 (90%).
- Demonstrates strong understanding of AWS storage concepts and EBS operations.

# 🎉 BONUS – AWS Cloud Foundations Completion

This section highlights the successful completion of the AWS Academy Cloud Foundations course, including certification and awarded badge.

---

## 🏅 AWS Academy Cloud Foundations Badge

![Badge AWS](https://github.com/user-attachments/assets/cec0b56c-952a-40dc-b289-64e92a6e23fe)


This badge represents the AWS Academy Cloud Foundations achievement, awarded for successfully completing the core cloud concepts course.

---

## 📜 AWS Academy Certificate of Completion

![Learners Lab Certificate](https://github.com/user-attachments/assets/ef7c3ee8-13ff-4a01-b439-e2571860fa83)


This certificate verifies completion of **AWS Academy Cloud Foundations**, including:
- **Course hours completed**: 20 hours
- **Issued on**: 06/23/2025







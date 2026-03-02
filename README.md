Project Overview

This project demonstrates a manual deployment of a static portfolio website inside a custom AWS VPC.



 Architecture Design

VPC CIDR: 10.0.0.0/16

Public Subnet: 10.0.1.0/24

Internet Gateway attached

Custom Route Table:

0.0.0.0/0 → IGW

EC2: Amazon Linux 2023 (t2.micro)

Web Server: Nginx

SSH restricted to personal IP

HTTP open to public

Network Flow

User Browser
    ↓
Public IP
    ↓
Internet Gateway
    ↓
Route Table
    ↓
Public Subnet
    ↓
EC2 (Nginx)

Security Considerations

SSH limited to my IP only


Default tenancy used

No IPv6 enabled

Key Learnings

Difference between public and private subnet

How route tables determine internet access

How Security Groups act as virtual firewalls

How EC2 receives both private and public IP

Linux file permissions and Nginx configuration



<img width="3839" height="1984" alt="image" src="https://github.com/user-attachments/assets/d81747bc-7a15-4787-a408-0d69b8d5de07" />


<img width="3839" height="2089" alt="image" src="https://github.com/user-attachments/assets/c90f7fe3-3e48-442e-995b-ffc91c6853b2" />

<img width="3839" height="1975" alt="image" src="https://github.com/user-attachments/assets/0c8372b8-bf6e-4e86-8adc-7b51709bd9d3" />

<img width="3840" height="1972" alt="image" src="https://github.com/user-attachments/assets/b2e4aaf2-7dd2-4529-a166-59ee64a15191" />

<img width="3839" height="1972" alt="image" src="https://github.com/user-attachments/assets/c4a529a6-d489-4cb0-98a3-04ab416110ef" />

<img width="3839" height="2069" alt="image" src="https://github.com/user-attachments/assets/09105bb7-ecdb-49c0-a42c-b4f4c2f98cb5" />





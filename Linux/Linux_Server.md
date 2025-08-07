# 🌐 Deploying a Linux Server on AWS EC2 with Basic Package Setup

## 🧾 Project Overview

This project demonstrates how to create a Linux-based EC2 instance on AWS, connect to it via SSH, and install essential packages such as `tree` and `nginx`. It serves as a foundational setup for hosting web applications or further DevOps projects.

---

## 🚀 Step-by-Step Guide

![Mobaxterm](/ScreenShot/Mobaxterm.png)

### ✅ Step 1: Launch an EC2 Instance

1. **Login to AWS Console**: [https://aws.amazon.com](https://aws.amazon.com)

![Acount](/ScreenShot/AWS-create.png)

![Signin](/ScreenShot/AWS-Signin.png)

2. **Navigate to EC2 Service**: Select **EC2** from the services list.
3. **Launch Instance**:

![Create instance](/ScreenShot/EC2.png)

   - Click **Launch Instance**

![Instance](/ScreenShot/Instance.png)

   - Name your instance (e.g., `Linux-Server`)
   - Choose **Amazon Linux 2023 AMI** or **Ubuntu Server 20.04 LTS**
   - Choose instance type (e.g., `t2.micro` - Free Tier eligible)
   - Select or create a key pair
   - Configure security group to allow **SSH (port 22)** and **HTTP (port 80)**
   - Click **Launch Instance**

![Lunch Instance](/ScreenShot/Create-Instance.png)



---

### ✅ Step 2: Connect to the Instance via SSH

```bash
# Set permissions and connect
chmod 400 your-key.pem
ssh -i "your-key.pem" ec2-user@<your-public-ip>
# OR for Ubuntu
ssh -i "your-key.pem" ubuntu@<your-public-ip>

```

![Key pair](/ScreenShot/key.png)

![Connect to Instance](/ScreenShot/connect.png)

---
## Package management

### Upadate the server 

![Update](/ScreenShot/update.png)
 
### Installed tree

![tree](/ScreenShot/tree.png)

### Upgrade the server

![upgrade](/ScreenShot/upgrade.png)

### Test tree 

![Tree](/ScreenShot/tree2.png)

### Delete tree 

![Delete tree](/ScreenShot/rm.png)

### Installed nginx

![Nginx](/ScreenShot/nginx.png)



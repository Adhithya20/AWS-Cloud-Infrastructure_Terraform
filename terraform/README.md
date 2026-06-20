# AWS-Cloud Infrastructure Terraform IaC
Automating AWS Cloud Infrastructure with Terraform — scalable, secure, and reproducible IaC
Here’s a professional **README.md** you can use for your *AWS Cloud Infrastructure — Terraform (IaC)* project. It’s structured in a way that works well on GitHub and makes your project easy to understand for recruiters, collaborators, or interviewers:

```markdown
# AWS Cloud Infrastructure — Terraform (IaC)

## 📌 Overview
This project demonstrates how to provision a **scalable, secure, and highly available cloud infrastructure** on Amazon Web Services (AWS) using **Terraform** as Infrastructure as Code (IaC).  
It automates the creation of a Virtual Private Cloud (VPC), subnets, Internet Gateway, NAT Gateway, EC2 instances, and an Application Load Balancer (ALB).

---

## 🚀 Features
- **VPC Setup**: Custom VPC with CIDR allocation.
- **Subnets**: Public and private subnets across multiple Availability Zones.
- **Internet Gateway & NAT Gateway**: Controlled inbound/outbound traffic.
- **EC2 Instance**: Amazon Linux 2 server with security groups for SSH (22) and HTTP (80).
- **Application Load Balancer (ALB)**: Distributes traffic across EC2 instances for high availability.
- **Security Groups**: Configured for least privilege access.
- **Terraform Outputs**: ALB DNS name and EC2 public IP for quick verification.

---

## 🛠️ Architecture
1. **VPC** with CIDR block `10.0.0.0/16`.
2. **Public Subnets** in two Availability Zones (`us-east-1a`, `us-east-1b`).
3. **Private Subnet** for backend resources.
4. **Internet Gateway** attached to the VPC.
5. **NAT Gateway** in a public subnet for private subnet outbound traffic.
6. **EC2 Instance** in a public subnet.
7. **Application Load Balancer** spanning two public subnets.
8. **Target Group & Listener** forwarding traffic to EC2.

---

## 📂 Project Structure
```
main.tf        # Terraform configuration
variables.tf   # Input variables (optional)
outputs.tf     # Outputs (ALB DNS, EC2 IP)
```

---

## ▶️ Usage
1. **Initialize Terraform**
   ```bash
   terraform init
   ```
2. **Validate configuration**
   ```bash
   terraform validate
   ```
3. **Apply changes**
   ```bash
   terraform apply
   ```
4. **Destroy infrastructure**
   ```bash
   terraform destroy
   ```

---

## 📊 Outputs
- **ALB DNS Name** → Access your application via the load balancer.
- **EC2 Public IP** → Direct access to the web server.

---

## ✅ Benefits
- Automated provisioning with Terraform.
- Consistent, reproducible environments.
- Scalable and highly available architecture.
- Easy teardown to avoid unnecessary costs.

---

## 📌 Author
**Adhithya P S**  
B.E. Computer Science Engineering | Cloud & DevOps Enthusiast  
```



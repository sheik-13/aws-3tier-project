# AWS 3-Tier Architecture Deployment Project

This project demonstrates the design and deployment of a **highly available, scalable, and secure 3-Tier architecture** on AWS, with separate **Web, Application, and Database tiers**. It was implemented as part of my AWS/DevOps learning journey.

---

## 🚀 Architecture Overview
- **Web Tier:** Public-facing EC2 instances behind an **External Application Load Balancer (ALB)**.
- **Application Tier:** Private EC2 instances behind an **Internal Load Balancer**, running Node.js app with PM2.
- **Database Tier:** Amazon RDS (MySQL) in private subnets, accessible only from the App Tier.

---

## 🔧 AWS Services Used
- **Compute:** EC2 (with Auto Scaling Groups)
- **Database:** Amazon RDS (MySQL)
- **Networking:** VPC, Subnets (Public/Private), Internet Gateway, NAT Gateway, Route Tables, Security Groups
- **Storage & IAM:** S3 (code storage), IAM Roles/Policies
- **Traffic Management:** Elastic Load Balancers (Internal & External), Route 53 (DNS)
- **Security & Delivery:** ACM (SSL), CloudFront (CDN with HTTPS)

---

## 🛠️ Key Configurations
- Configured **5 VLANs** for segmentation (for CCNA project reference).
- Used **DHCP and ACLs** for VLANs, restricting access and enabling controlled communication.
- Deployed **CI/CD pipelines** with Ansible + GitHub for automation.
- Configured **health checks** (`/health`) for monitoring EC2 instances.
- Applied **least-privilege IAM roles** for EC2-to-S3 access.

---

## 📌 Highlights
- Reduced deployment time by **80%** with automation.
- Achieved **secure global delivery** using CloudFront + ACM.
- Validated **end-to-end connectivity** (Web → App → DB).

---

## 📂 Files in This Repository
- `AWS-project-preparation.docx` → Detailed step-by-step documentation of the project.  
- `README.md` → This documentation file.  

---

## 🔗 Related Projects
- **CCNA Networking Project – VLAN & Server Configuration**  
Designed a multi-VLAN college network using Cisco Packet Tracer with **DHCP, ACLs, VLAN trunking**, and server access control.  

---

## 👤 Author
**Sheik Mohamed P**  
- 📧 Email: sheikmohamed77089@gmail.com  
- 🌐 LinkedIn: www.linkedin.com/in/sheik-mohamed-5893b1261  
- 💻 GitHub: https://github.com/sheik-13 


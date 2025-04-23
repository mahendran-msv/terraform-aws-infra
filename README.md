# 🚀 Terraform AWS Infrastructure Deployment

This project demonstrates Infrastructure as Code (IaC) using **Terraform** to provision a scalable and highly available **AWS infrastructure** with automated deployments using **GitHub Actions CI/CD**.

## 🔧 What This Project Builds

- **VPC** with public and private subnets
- **Internet Gateway** for public subnet access
- **NAT Gateway** for internet access from private subnets
- **Route Tables** for traffic management
- **Application Load Balancer (ALB)** in public subnets
- **Auto Scaling Group (ASG)** with EC2 instances in private subnets
- **S3 Bucket** for remote Terraform state with **DynamoDB locking**
- **Security Groups** for controlled access

## 🛠️ Tools & Technologies

- **Terraform** (v1.5+)
- **AWS** (EC2, VPC, ALB, ASG, S3, IAM, CloudWatch)
- **GitHub Actions** for CI/CD
- **S3 + DynamoDB** for remote backend
- **Bash** for helper scripts (optional)

## 🧩 Project Structure

(See folders and files in the repo)

## ⚙️ CI/CD with GitHub Actions

Automated via GitHub Actions to run:
- `terraform fmt`
- `terraform validate`
- `terraform plan`

## 🔒 Remote State Configuration

State files stored in an **S3 bucket** with **DynamoDB table** for locking.

## ✅ How to Use

```bash
git clone https://github.com/your-username/terraform-aws-infra.git
cd terraform-aws-infra/environments/dev
terraform init
terraform plan
terraform apply
```

## 👤 Author

**Mahendran Govindaraju**  
[AWS & DevOps Engineer](mailto:gmahendran606@gmail.com)

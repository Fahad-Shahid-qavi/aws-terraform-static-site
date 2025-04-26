**Static Website Hosting on AWS using Terraform**

**🔥 About the Project**

This project demonstrates how to deploy a secure, scalable static website using AWS and Terraform.

Website content is stored in a private S3 bucket.
Content is delivered globally and securely using CloudFront.
Infrastructure is fully automated through Infrastructure as Code (IaC) with Terraform.
The goal is to showcase practical skills in cloud architecture, automation, and best practices for modern web hosting.

**🛠 Technologies Used**

AWS S3 — Storage for static website files
AWS CloudFront — Global Content Delivery Network (CDN) for fast, secure delivery
Terraform — Infrastructure as Code tool for automating AWS resource creation

**📂 Project Structure**

main.tf — Defines all AWS resources (S3 bucket, CloudFront distribution, security policies)
variables.tf (optional) — Input variables to make the configuration reusable
outputs.tf (optional) — Outputs important information like the CloudFront URL after deployment

**🚀 How to Deploy**

1- Clone the Repository
    git clone <your-repo-url>
    cd <your-project-folder>

2- Set Up AWS Credentials Make sure the AWS CLI is configured with appropriate permissions:
    aws configure
    
3- Initialize Terraform Install the required providers and set up the environment:
    terraform init
    
4- Preview Changes Review what resources will be created:
    terraform plan
    
5- Deploy Infrastructure Create the AWS resources:
    terraform apply
    
6- Confirm by typing yes when prompted.

7- Upload Website Files Upload your static site files (e.g., index.html) to the S3 bucket:
    aws s3 cp ./index.html s3://<your-s3-bucket-name>/
    
8- Access Your Website Once deployed, the CloudFront distribution URL will serve your website over HTTPS.

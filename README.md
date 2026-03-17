# AWS Static Website Deployment with CI/CD

## Overview
This project demonstrates how to deploy a static website on AWS using Amazon S3 and deliver it globally using Amazon CloudFront. It also includes a CI/CD pipeline using GitHub Actions to automate deployments.

## Architecture
The solution follows a simple cloud architecture:

User → CloudFront → S3

- Amazon S3 stores and hosts static website files
- Amazon CloudFront distributes content globally with low latency
- GitHub Actions automates deployment to S3 on every code push

## Technologies Used
- Amazon S3
- Amazon CloudFront
- GitHub
- GitHub Actions

## Features
- Static website hosting on AWS
- Secure content delivery via HTTPS
- Automated deployment pipeline
- Global content distribution

## Deployment Workflow
1. Developer pushes code to GitHub repository
2. GitHub Actions workflow is triggered
3. Files are synced to the S3 bucket
4. CloudFront serves updated content


## Setup Instructions

### 1. Create S3 Bucket
- Enable static website hosting
- Upload website files
- Configure public access

### 2. Configure CloudFront
- Set S3 website endpoint as origin
- Enable HTTPS redirection
- Set default root object to index.html

### 3. Configure CI/CD
- Create GitHub repository
- Add AWS credentials as secrets
- Add GitHub Actions workflow

## Repository
https://github.com/IPOUL2208/aws-static-site-devops

## Future Improvements
- Infrastructure as Code using Terraform
- Custom domain with Route 53
- Monitoring with CloudWatch

## Author
IPOUL2208

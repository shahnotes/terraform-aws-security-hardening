# 🛡️ Terraform AWS Security Hardening

![Terraform](https://img.shields.io/badge/Terraform-v1.x-blueviolet?logo=terraform)
![AWS](https://img.shields.io/badge/AWS-Deployed-orange?logo=amazon-aws)
![CI/CD](https://img.shields.io/github/actions/workflow/status/shahnotes/terraform-aws-security-hardening/github-actions.yaml?label=CI%2FCD&logo=github)
![Security Scanning](https://img.shields.io/badge/Scanned%20by-tfsec%20%26%20Checkov-blue?logo=datadog)
![Stars](https://img.shields.io/github/stars/shahnotes/terraform-aws-security-hardening?style=social)

> **Automated Security Hardening Pipeline** using Terraform, GitHub Actions, and AWS native security tools.  
> Infrastructure-as-Code meets DevSecOps — built to secure, scale, and stay compliant.

---

## 🚀 Overview

This project automates the provisioning and security hardening of AWS infrastructure using **Terraform** and a **CI/CD pipeline with built-in security checks**. It's designed for teams and cloud engineers who want to deploy production-grade, secure-by-default environments — without compromising on automation.

✅ IaC best practices  
✅ Terraform scanning with `tfsec` and `checkov`  
✅ GitHub Actions CI/CD integration  
✅ Encryption, logging, least privilege IAM  
✅ AWS Config, GuardDuty, CloudTrail, Security Hub ready  
✅ Modular, scalable, and reusable

---

## 📐 Architecture

```plaintext
┌──────────────┐
│   GitHub     │
└────┬─────────┘
     │ Push/PR
     ▼
┌──────────────┐     ┌──────────────────┐
│ GitHub CI/CD ├────▶ Terraform + Scans │
└────┬─────────┘     └────┬─────────────┘
     │                    │
     ▼                    ▼
┌──────────────┐    ┌────────────────────┐
│ AWS Infra    │    │ Security Tools     │
│ (VPC, EC2,…) │    │ tfsec, checkov     │
└──────────────┘    └────────────────────┘

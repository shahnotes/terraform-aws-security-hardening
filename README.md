# 🛡️ Terraform AWS Security Hardening

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
│ GitHub CI/CD ├────▶ Terraform + Scans│
└────┬─────────┘     └────┬─────────────┘
     │                    │
     ▼                    ▼
┌──────────────┐    ┌────────────────────┐
│ AWS Infra    │    │ Security Tools     │
│ (VPC, EC2,…) │    │ tfsec, checkov     │
└──────────────┘    └────────────────────┘
# ☁️ AWS Brand New Account Setup — Secure Cloud Foundation  
A step-by-step guide to building a **secure, professional AWS account** from scratch — designed for learning, certifications, and portfolio projects.

---

## 🧭 Overview
This project demonstrates how to configure a new AWS account following **real-world best practices** in security, billing control, and account organization.  
The goal is to replicate how a Solutions Architect would set up a fresh environment for hands-on labs or client onboarding — with documentation clear enough for others to follow.

---

## 🧰 Objectives
- Establish a **clean, isolated AWS account** for experimentation and demos.  
- Implement **root account security** (MFA, no access keys).  
- Configure **budget alerts** and **Free Tier safeguards**.  
- Create **IAM administrative access** with least-privilege principles.  
- Build a **documented project structure** for screenshots, notes, and reusable templates.

---

## 🗂️ Project Structure
```
brand-new-aws-setup-guide/
├─ README.md          ← main documentation
├─ notes/             ← written explanations or configs
├─ screenshots/       ← setup visuals
└─ resources/         ← references, PDFs, budgets
```
---

## ⚙️ Stage 1 — Account Creation
A new AWS account is created using a **dedicated email** and verified payment method. Simply instead of using personal email, just create new one dedicated only for AWS example: aws.labs.yourname@gmail.com.
The account is set to **Basic (Free)** support with region **N. Virginia (us-east-1)** for maximum service availability.  
Only the root user is active at this stage and will later be secured and replaced by IAM administrators.

**Key actions**
- Registered a separate AWS-only email address.  
- Completed contact, verification, and payment setup (temporary $1 authorization).  
- Selected *Basic (Free)* support plan.  
- Logged in as root user and confirmed default region **us-east-1**.

**Outcome**
- A clean, verified AWS root account ready for hardening and IAM configuration.  
- Root login reserved strictly for billing and recovery tasks.

---

## 📈 Upcoming Stages
| Stage | Description |
|-------|--------------|
| **2. Root Hardening** | Enable MFA, remove root access keys, set recovery options. |
| **3. Billing Controls** | Configure $5 budget, Free Tier alerts, enable Cost Explorer. |
| **4. IAM Admin Setup** | Create admin user, assign AdministratorAccess, manage keys. |
| **5. Project Structure** | Build S3 bucket `aws-account-setup-docs`, add tagging standards. |
| **6. Verification** | Validate Free Tier, confirm billing $0, finalize documentation. |

---

## 🧠 Professional Insight
This repository highlights essential **security and governance discipline** in cloud environments.  
Clear documentation, separation of duties, and proactive billing controls are cornerstones of AWS best practices — valuable for roles in **Cloud Security, DevSecOps, and Architecture**.

---

## 🔖 Tags
`#AWS` `#CloudSecurity` `#SolutionsArchitect` `#DevSecOps` `#BeginnerProject`

---

### © 2025 Aykhan Pashayev  
Created for educational and professional portfolio use.  
Part of a larger initiative to document secure, reproducible AWS architectures.

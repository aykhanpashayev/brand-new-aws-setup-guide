# 🧱 AWS Account Setup Guide  
**Author:** Aykhan Pashayev  
**Project Type:** Foundational AWS configuration & documentation  
**Goal:** Build a **secure, isolated AWS environment** for learning, certification labs, and portfolio projects — configured to professional standards and fully documented step by step.  

---

## 📘 Project Overview  
This repository documents the full lifecycle of setting up a brand-new AWS account from scratch — exactly as a cloud engineer or solutions architect would do for a sandbox or demo environment.  

Each stage follows a consistent structure:  
- **Objective:** what & why  
- **Console path / URL:** where to click  
- **Actions:** numbered steps  
- **Expected confirmation:** what success looks like  
- **Screenshot / note instructions**  
- **GitHub Log Note:** short summary for version control  

💡 **Purpose:**  
Many beginners skip the foundational setup and jump straight into services.  
This guide ensures every account is configured safely — with proper billing controls, MFA, IAM separation, tagging, and documentation — just like a production-grade environment.

---

## 🧩 Project Folder Structure
AWS-Account-Rebuild/
├── README.md ← main documentation (this file)

├── notes/ ← written explanations or configs

├── screenshots/ ← redacted images per stage

└── resources/ ← reference files, PDFs, budgets, etc.

---

## ⚙️ Recommended Tools Before You Start
| Tool | Purpose |
|------|----------|
| **Password Manager** (Bitwarden, 1Password, etc.) | Securely store root & IAM credentials |
| **MFA App** (Authy / Google Authenticator) | Protect email and AWS root login |
| **Browser Profiles** (Chrome → Profile > Add) | Keep AWS work separate from personal browsing |
| **Cloud Notebook** (CherryTree / Obsidian / Notion) | Keep quick setup notes |
| **GitHub Account** | For version-controlling this documentation |

---

## 🧭 Stage 1 – Create a Dedicated AWS Account

### 🎯 Objective
Create a **brand-new AWS root account** that’s completely isolated from your personal one.  
This will be your long-term lab and portfolio environment.  
The key principle is **separation of concerns** — never mix production, study, or sandbox resources under one billing identity.

---

### 🔗 Console Paths
Sign-up: https://portal.aws.amazon.com/billing/signup

Root sign-in: https://console.aws.amazon.com/

---

### 🪜 Steps

1. **Create a dedicated email**  
   - Use an email reserved only for AWS projects.  
     Example: `aws.labs.aykhan@gmail.com`  
   - 💡 For multiple environments later, use Gmail “+” aliases (`aws.labs+dev@…`, `aws.labs+test@…`).  
   - Enable MFA on that email account first.  

2. **Start AWS sign-up**  
   - Go to the Sign-up link.  
   - Choose **Personal Account**.  
   - Enter the dedicated email, strong password, and account name (e.g., `Aykhan-Labs`).  

3. **Provide contact details**  
   - Select your country, enter full name, address, and phone.  
   - Keep **Account Type: Personal** (simpler for lab billing).  

4. **Add payment method**  
   - Enter a valid debit/credit card.  
   - AWS may hold **$1 USD** temporarily for verification.  

5. **Verify identity**  
   - Choose **SMS** or **Voice Call**, complete verification code.  

6. **Select support plan**  
   - Choose **Basic (Free)**.  

7. **Confirm email verification**  
   - Check inbox for “Welcome to Amazon Web Services.”  
   - Confirm the link if prompted.  

8. **Sign in as root**  
   - Use the Root sign-in link above.  
   - Sign in with the email (not an IAM user).  

9. **Choose primary region**  
   - In AWS Console → top-right Region dropdown → select **N. Virginia (us-east-1)**.  
   - 💡 Widest service availability and best for docs and labs.  

10. **Verify console access**  
    - You should now see the AWS Management Console home page with your account name in the top-right menu.  

---

### ✅ Expected Confirmation
- You receive AWS welcome/verification emails.  
- You can access Billing Console and AWS Console Home without errors.  
- Region = **N. Virginia (us-east-1)** is visible.  

---

### 🧾 Security & Best-Practice Notes
| Area | Recommendation |
|------|----------------|
| **Root email** | Use only for billing & critical tasks |
| **Browser** | Use a separate profile labeled “AWS Root” |
| **Passwords** | Store securely in a password manager |
| **Shared devices** | Never sign in to AWS root on public machines |
| **Future stages** | Root login will be locked down; daily use moves to IAM Admin user |

---

### 💬 GitHub Log Note

# 🔐 AWS IAM (Identity and Access Management)

AWS IAM is a service that helps you **secure and manage access** to your AWS resources.  
Think of it like a security system for your AWS account.

IAM lets you:
- 👤 Create users
- 👥 Group users with similar access
- 🎭 Assign roles for temporary access
- 📜 Define what users can or can’t do using policies

IAM follows the **least privilege principle** — only give users the permissions they need.

---

## 🧱 Components of IAM

### 👤 Users
- IAM users are people or applications that need to interact with AWS.
- Each user has a unique name and login credentials (password or access keys).
- Users should only get the access they need — no more.

---

### 👥 Groups
- Groups are **collections of users** with the same access needs.
- You attach policies to the group instead of each user.
- When a user is added to a group, they get the group's permissions.

---

### 🎭 Roles
- Roles are used to give **temporary access** to AWS services or users.
- Commonly used by applications or services to access resources **without a password**.
- Roles come with permissions defined in policies.

---

### 📜 Policies
- Policies are written in **JSON format** and define what actions are allowed or denied.
- You can attach policies to users, groups, or roles.
- Policies control access to AWS services like S3, EC2, Lambda, etc.

**Types of Policies:**
- ✅ **AWS Managed Policies** – ready-made by AWS
- 🛠️ **Customer Managed Policies** – you create and manage these yourself

---

## 🔐 Security Features

- 🔑 IAM supports **Multi-Factor Authentication (MFA)** for added login security.
- 📈 It provides an **audit trail** of user activity and permission changes.
- 🔍 Everything is **logged**, so you know who did what and when.

---

## ✅ Best Practices

- Use **MFA** for root and IAM users
- Grant **least privilege** permissions
- Avoid using the **root account** for daily tasks
- Regularly review permissions and activity

---

## 🧠 Summary

IAM is your **security and access manager** in AWS.

It ensures that:
- ✅ Only the right people have access
- 🚫 Unwanted access is blocked
- 🛡️ Everything is monitored and secure

> 🔒 **By using IAM wisely, you protect your cloud environment and control access properly.**


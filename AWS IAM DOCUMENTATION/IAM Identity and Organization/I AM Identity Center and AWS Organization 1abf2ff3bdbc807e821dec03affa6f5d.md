# I AM Identity Center and AWS Organization

## What is the I AM Identity Center?

**IAM Identity Center** is a service that helps manage access to AWS accounts and applications using **single sign-on (SSO)** and centralized identity management. It allows organizations to control user access efficiently across multiple AWS accounts and business applications.

AWS **IAM Identity Center** is responsible for **creating users and groups and granting permissions. It allows users** to **log in and access multiple AWS accounts within an AWS Organization** using a single sign-in.

## **What Does AWS Identity Center Do?**

AWS **Identity Center (formerly AWS SSO)** is a **centralized identity and access management service** that allows users to securely access multiple AWS accounts and applications **with a single login**.

## **Key Functions of AWS Identity Center**

**1: Single Sign-On (SSO):** Users can log in once and access multiple AWS accounts without needing multiple passwords.

**2: Centralized User Management:** It controls which users can access which AWS accounts and services.

3: Integration with External Identity Providers (IdP): This integrates with **Microsoft Entra ID (Azure AD), Okta, Google Workspace**, and other IdPs.

4: **Enforces Security Policies:** Ensures users have the right level of access based on permissions.

**5: Manages Access to AWS and Third-Party Apps:** Grants access to AWS Management Console, CLI, and supported SaaS applications.

## **What is an AWS Organization?**

**AWS Organizations** is a service that **helps businesses create and manage multiple AWS accounts** in a structured and centralized way. It enables **billing consolidation, security policy enforcement, and access management** across all linked accounts.

**Key Features of an AWS Organization**

1: **Centralized Account Management:** Organizes multiple AWS accounts under a single structure.

**2: Billing Consolidation:** Combines all AWS bills into one for cost tracking and discounts.

3: **Security and Compliance:** Uses **Service Control Policies (SCPs)** to enforce security rules across accounts.

4: **Access Control:** Works with AWS **Identity Center (SSO)** for centralized user authentication.

5: **Delegated Administration:** Can assign specific accounts to manage IAM, security, and access policies.

![image.png](image.png)

# **Steps to Create an AWS Organization**

### **1: Sign in to AWS as the Root User**

- Go to the [AWS Management Console](https://aws.amazon.com/console/).
- Sign in using the **root user** of the AWS account you want to be the **Management Account**.

![image.png](image%201.png)

### **2: Navigate to AWS Organizations**

- In the AWS Management Console, search for and select **"AWS Organizations"**.
- Click **“Create an Organization”**.

![image.png](image%202.png)

### **3: Enable I AM  Identity Center**

- Go to I AM Identity Center
- Click **"Enable"**.
- Confirm your identity source
- Manage permissions for multiple users

![image.png](image%203.png)

![image.png](image%204.png)

![image.png](image%205.png)

![image.png](image%206.png)

![image.png](image%207.png)

### **4: Add AWS Accounts to the Organization**

You can now invite or create new AWS accounts to be part of your organization:

 **Option 1: Invite Existing AWS Accounts**

- Click **"Add an AWS Account"** → **"Invite an AWS account"**.
- Enter the **AWS account email or account ID**.
- Send the invitation; the invited account owner must accept.

![image.png](image%208.png)

![image.png](image%209.png)

![image.png](image%2010.png)

**Option 2: Create a New AWS Account**

- Click **"Add an AWS Account"** → **"Create an AWS account."**
- Enter the **account name and email**.
- AWS will send an email to verify the account.

![image.png](image%2011.png)

![image.png](image%2012.png)

![image.png](image%2013.png)

## What is a CloudTrail?

**AWS CloudTrail** is a service that records **all actions (API calls) made in an AWS account** and provides a history of events for security, compliance, and troubleshooting. It is a service that tracks user activity and API usage for AWS accounts.

### **Key Features of AWS CloudTrail**

**1: Tracks AWS API Calls:** Logs who did what, when, and from where.

**2: Stores Event History:** Saves logs in **Amazon S3** for security audits.

3: **Detects Unauthorized Access: Helps** identify suspicious activities.

**4: Integrates with AWS Security Tools** Works with **AWS CloudWatch** and **AWS Security Hub** for monitoring.

### **Why is AWS CloudTrail Important?**

**Security and Compliance:** Ensures accountability by logging all AWS actions.

**Troubleshooting:** Helps diagnose operational issues.

**Audit Readiness:** Meets industry compliance standards like **ISO, PCI-DSS, and HIPAA**.

[How to create Azure cloud and use Entra ID to manage users, groups, and policies](https://www.notion.so/How-to-create-Azure-cloud-and-use-Entra-ID-to-manage-users-groups-and-policies-1acf2ff3bdbc80cc818ef53f34e11d28?pvs=21)
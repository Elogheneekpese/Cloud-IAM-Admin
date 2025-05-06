# Understanding AWS Users, Groups, and Policies: A Simple Guide. (1)

If you've ever used AWS, you know it can feel like a giant maze of services, permissions, and security settings. One of the most important things to get right from the start is user management—who gets access to what and how you control it.

Let’s break it down without the tech jargon and make it easy to understand.

![image.png](image.png)

# **Identity and Access Management (IAM) Lifecycle**

Identity and Access Management (IAM) is a framework of policies and technologies that ensures the right individuals have appropriate access to resources within an organization. The IAM lifecycle consists of several key stages that maintain security, efficiency, and compliance.

## **1. Provisioning**

Provisioning is the process of creating and assigning digital identities to users when they join an organization. This includes:

- Creating a user account with a unique identifier.
- Assigning roles, permissions, and access rights based on job responsibilities

## **2. Authentication**

Authentication is the process of verifying a user’s identity before granting access. Common authentication methods include:

- **Multi-Factor Authentication (MFA):** requires additional verification like OTPs, biometrics, or security tokens.
- **Single Sign-On (SSO):** allows users to access multiple applications with one login.

## **3. Authorization**

Authorization determines what resources a user can access after authentication. This is typically managed through:

- **Role-Based Access Control (RBAC):** Users are assigned roles with predefined permissions.

## **4. Self-Service**

Self-service IAM features empower users to manage their own identities by

- **Profile updates:** Users can update their details (e.g., phone number, email).
- **Access requests:** Employees can request access to new resources with approval workflows.

## **5. Password Management**

Password management involves enforcing strong authentication policies to protect user accounts. This includes:

- **Enforcing strong passwords:** using complexity rules (length, special characters, etc.).
- **Regular password rotation:** encouraging users to update passwords periodically.

## **6. Governance**

IAM governance ensures compliance with security policies and regulations. This includes:

- **User access reviews:** periodic audits to verify that access permissions are appropriate.
- **Compliance monitoring:** ensuring adherence to frameworks like GDPR, HIPAA, and ISO 27001.
- **Identity analytics:** monitoring and detecting suspicious activities to prevent security breaches.

## **7. Deprovisioning**

Deprovisioning is the process of revoking access when a user leaves the organization or changes roles. Steps include:

- **Disabling or deleting user accounts:** ensuring no unauthorized access.
- **Revoking access to systems, applications, and sensitive data**.
- **Reassigning licenses and resources—o**ptimizing IT resource management.

**Imagine AWS as a massive corporate building with different departments, employees, and security access levels. Not everyone should have the keys to every room, right? That’s where Users, Groups, and Policies come in.**

---

## **Who Are AWS Users? Employees in the Office**

AWS **Users** are like employees in a company. Each one has a unique identity (username + password) and is given access to specific areas of the building (AWS services).

 **Example:**

- A **developer** might need access to EC2 (virtual machines).
- A **finance team member** may only need access to billing reports.
- A **support engineer** might only access AWS logs to troubleshoot issues.

How **Do You Create an AWS User?**

1: Go to **AWS IAM (Identity and Access Management)**.

2: Click **Users → Add User**.

3: Done! The user can now log in with their credentials.

![image.png](image%201.png)

![image.png](image%202.png)

## **What Are AWS Groups? Departments in the Office**

AWS **Groups** are like departments in the company. Instead of assigning permissions to each user one by one (which gets messy), you group users and give them shared access.

**Example:**

- **Developers Group** → Access to EC2, S3, Lambda
- **Finance Group:** Access to Billing
- **Support Team** → Read-only access to logs

**How to Create a Group in AWS IAM?**

1: Go to **AWS IAM → Groups → Create Group**.

2: Add users who should be in this group.

3: Attach policies (explained next!).

4:Done! Everyone in the group gets the assigned permissions.

![image.png](image%203.png)

![image.png](image%204.png)

![image.png](image%205.png)

**What Are AWS Policies? (Security Access Badges in the Office)**

Policies are like **access badges** in our office analogy. They define **what a user or group is allowed to do** in AWS.

**Example Policies:**

- **AdministratorAccess:** Full control of everything
- **ReadOnlyAccess:** Can view everything but can’t make changes 👀
- **EC2FullAccess** → Can create, modify, and delete EC2 instances

AWS Policies use JSON (a coding format), but don’t worry—you **don’t need to write code** to apply them. You can use AWS-managed **policies** (pre-made templates) or create custom ones.

1: Go to **AWS IAM → Policies Create Policy** (or choose an existing one).

2: Select a **user or group** to apply it to.

3: Done! The permissions are now active.

![image.png](image%206.png)

![image.png](image%207.png)

AWS **Users, Groups, and Policies** are the foundation of **cloud security and access management**. By understanding how they work, you ensure **your AWS environment stays organized, secure, and efficient**.
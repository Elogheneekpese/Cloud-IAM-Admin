# How to create Azure cloud and use Entra ID to manage users, groups, and policies

**Azure** is a **cloud computing platform** and **service provider** created by **Microsoft**. It offers a wide range of **cloud services** for computing, storage, networking, databases, AI, security, and more.

### **Key Features of Azure as a Cloud Provider:**

**Infrastructure as a Service (IaaS):** Virtual machines, storage, networking

 **Platform as a Service (PaaS):** Web apps, databases, and DevOps tools

 **Software as a Service (SaaS)** : Microsoft 365, Dynamics 365

**Identity and Security**: Azure Active Directory (now **Entra ID**), IAM, MFA, Zero Trust

## What is Entra ID?

"Entra ID manages user identities, groups, and permissions, enabling secure authentication and access control across cloud and on-premises environments.

### **Key Features of Entra ID:**

 **Identity Management** – Manages users, groups, and permissions.

 **Single Sign-On (SSO)** – Allows users to access multiple applications with one login.

 **Multi-Factor Authentication (MFA)** – Adds extra security beyond passwords.

 **Conditional Access** – Controls access based on user, device, and location.

 **Identity Governance** – Automates access reviews, role assignments, and lifecycle policies.

**Integration with Microsoft & Third-Party Apps:** Works with Microsoft 365, Azure, AWS, Okta, and other SaaS apps.

## Creating an Azure cloud:

**1. Create an Azure account:**

- **Go to the Azure portal:** Start by navigating to the official Microsoft Azure website (portal.azure.com).
- **Provide necessary information and sign up for a free account:** You will need to provide your email address, phone number, and payment information.

**2. Navigate the Azure Portal:**

- **Familiarize yourself with the dashboard:** Once logged in, you'll see the Azure dashboard. This is your central hub for managing Azure resources.

![image.png](image.png)

## **These are the steps to creating an organization account below**

1. Domain verification
2. Setting primary domain   
3. Creating users/bulk users
4. Create groups
5. Permissions

Now, lets dive into the above with our pictorial illustrations

## A: Domain Verification

1. Log in to Microsoft Azure account
2. Click on Microsoft Entra ID
3. Click on manage and expand it
4. Click on Custom domain names
5. Cick on add custom domain

![image.png](image%201.png)

![image.png](image%202.png)

1. Go to your domain website and verify the above TXT records

![image.png](image%203.png)

![image.png](image%204.png)

## B: Setting primary domain

1: Go to custom domain names

2: Click on the name you want to make a primary domain

3: Go to overview and refresh 

![image.png](image%205.png)

![image.png](image%206.png)

![image.png](image%207.png)

## C: Creating of users/bulk users

1: Click on users

2: Click on add new user

3: Click on either create user or invite external user

3i: Create new user

![image.png](image%208.png)

3ii: Create an external user

![image.png](image%209.png)

3iii: Create bulk users

Click on bulk operations, then bulk create

![image.png](image%2010.png)

![image.png](image%2011.png)

# D. Creating of groups

1. Click on groups
2. Click on new group

![image.png](image%2012.png)

1. Refresh and click on all groups

![image.png](image%2013.png)

![image.png](image%2014.png)

### E. Assigning of permissions to users and groups

![image.png](image%2015.png)

1. Click on users
2. Click on the user you want to assign a role
3. Click on assigned roles
4. Click on add  assignments

![image.png](image%2016.png)

![image.png](image%2017.png)

Assigning permission to a group

1. Click on groups
2. Click new group

![image.png](image%2018.png)

1. Click on all groups
2. Click on the new group created
3. Click on manage to expand 
4. Then assign permission

## Azure cloud and microsoft Entra ID Permissions

### **Why Do Microsoft Entra ID and Azure Cloud Have Separate Permissions?**

While **Microsoft Entra ID** (formerly Azure AD) and **Azure Cloud** are deeply integrated, they handle **different aspects of security and access control**, which is why they run separate permission models.

### **Key differences in permissions:**

| Feature | **Microsoft Entra ID** | **Azure Cloud (RBAC)** |
| --- | --- | --- |
| **Focus** | Identity & Authentication | Resource & Infrastructure Access |
| **Controls** | Who can log in & what apps they can access | What actions users can perform on Azure services |
| **Roles** | Global Admin, User Admin, Security Admin | Owner, Contributor, Reader, Custom Roles |
| **Scope** | Organization-wide (across multiple platforms) | Azure-specific resources (VMs, storage, databases) |

Now, using illustrations to assign permission to a user through Azure cloud in order to access cloud resources.

1. After creating a user in Entra ID
2. Log into Azure portal and click on subscription
3. Click on Azure subscription 1
4. Click on Access control ( IAM )
5. Click on add role assignment
6. 

![image.png](image%2019.png)

![image.png](image%2020.png)

![image.png](image%2021.png)

![image.png](image%2022.png)

![image.png](image%2023.png)

![image.png](image%2024.png)

![image.png](image%2025.png)

![image.png](image%2026.png)

![image.png](image%2027.png)
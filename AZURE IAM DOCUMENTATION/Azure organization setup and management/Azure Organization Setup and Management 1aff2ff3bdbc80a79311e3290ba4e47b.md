# Azure Organization Setup and Management

## **A. Introduction**

An **Azure Organization** refers to an **Azure Active Directory (Azure AD) tenant** that businesses use to manage identities, users, and resources within Microsoft Azure. It serves as the foundation for identity and access management in an enterprise, allowing organizations to secure their cloud environment, control user permissions, and integrate with Microsoft services like Microsoft 365, Dynamics 365, and Azure subscriptions.

### **Why Create an Azure Organization?**

1. Centralize identity management with **Azure Active Directory (Azure AD)**.
2. Securely manage users, groups, and permissions with **Role-Based Access Control (RBAC)**.
3. Provide seamless authentication for employees and external users.
4. Integrate cloud-based applications and services efficiently.
5. Ensure compliance and enforce security policies with m**ulti-factor authentication (MFA)** and c**onditional access**.

---

## **B. Steps to Create an Azure Organization**

### **Step 1: Sign Up for an Azure Account**

1. Visit Azure Portal.
2. Click **"Start Free"** (if creating a new Azure account) or **"Sign in"** (if you already have a Microsoft account).
3. Enter your Microsoft account, GitHub account, or a work or school account and follow the prompts.

 Using your work or school account automatically connects your organization to your Microsoft Entra ID.

### **Step 2: Configure the Organization Details**

1. Once logged in
2. Go to Microsoft 365 Copilot/Microsoft 365 Business plan page
3. Select “buy Microsoft 365.”
4. Enter a name for your organization (e.g., "YourCompany Ltd").
5. Choose a primary domain name (e.g., `yourcompany.onmicrosoft.com`).
6. Select the country or region where your organization operates.

![image.png](image.png)

![image.png](image%201.png)

![image.png](image%202.png)

![image.png](image%203.png)

### **Step 3: Add Users and Assign Roles**

1. In Azure AD > Users, click New user to add employees.
2. Assign roles (e.g., Global Admin, User, Billing Administrator).
3. Save changes and notify users of their login credentials.

![image.png](image%204.png)

![image.png](image%205.png)

![image.png](image%206.png)

![image.png](image%207.png)

![image.png](image%208.png)

### **Step 4: Add a Custom Domain (Optional)**

1. Navigate to Azure AD > Custom domain names.
2. Click Add custom domain and enter your company domain (e.g., `yourcompany.com`).
3. Follow the instructions to verify domain ownership via DNS settings.

![image.png](image%209.png)

![image.png](image%2010.png)

### **Step 5: Assign a License**

- Go to Microsoft 365 Admin center
- Click on users
- Click on active users
- Click on the name of the user to license
- Click on License and app
- Click Save to apply the license.
- Choose the subscription or license plan
- Click save to apply

![image.png](image%2011.png)

![image.png](image%2012.png)

![image.png](image%2013.png)

![image.png](image%2014.png)
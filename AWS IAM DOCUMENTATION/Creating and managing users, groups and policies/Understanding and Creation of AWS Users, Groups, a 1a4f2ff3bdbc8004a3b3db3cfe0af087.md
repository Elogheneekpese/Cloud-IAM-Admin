# Understanding and Creation of AWS Users, Groups, and Policies: A Simple Guide.

If you've ever used AWS, you know it can feel like a giant maze of services, permissions, and security settings. One of the most important things to get right from the start is user management—who gets access to what and how you control it.

Let’s break it down without the tech jargon and make it easy to understand.

## **First, Think of AWS Like a Big Office Building**

Imagine AWS as **a massive corporate building** with different departments, employees, and security access levels. Not everyone should have the keys to every room, right? That’s where **Users, Groups, and Policies** come in.

---

## **Who Are AWS Users? Employees in the Office**

AWS **Users** are like company employees. Each one has a unique identity (username + password) and is given access to specific areas of the building (AWS services).

Example:

- A **developer** might need access to EC2 (virtual machines).
- A **finance team member** may only need access to billing reports.
- A **support engineer** might only access AWS logs to troubleshoot issues.

How **Do You Create an AWS User?**

1: Go to **AWS IAM (Identity and Access Management)**.

2: Click **Users → Add User**.

3: Done! The user can now log in with their credentials.

![image.png](image.png)

![image.png](image%201.png)

**Creating an I AM User that can log in through the web console**

**Step 1: Create a New IAM User**

1. In the **IAM Console**, click on **Users.**
2. Click the **"create users"** button.
3. Enter a **username** (e.g., Mercy)
4. Then review and create.
    - For this I AM user to have access to the AWS console, then go to security credentials and enable the console and custom-fill out the password
    - Then you can log in with your details to access the AWS console, but this time through I AM User

![image.png](image%202.png)

![image.png](image%203.png)

![image.png](image%204.png)

**What Are AWS Groups? Departments in the Office**

AWS **Groups** are like departments in the company. Instead of assigning permissions to each user one by one (which gets messy), you group users and give them shared access.

**Example:**

- **Developers Group** → Access to EC2, S3, Lambda
- **Finance Group** → Access to Billing
- **Support Team** → Read-only access to logs

**How to Create a Group in AWS IAM?**

1: Go to **AWS IAM → Groups → Create Group**.

2: Add users who should be in this group.

3: Attach policies (explained next!).

4:Done! Everyone in the group gets the assigned permissions.

![image.png](image%205.png)

![image.png](image%206.png)

![image.png](image%207.png)

![image.png](image%208.png)

**What Are AWS Policies? (Security Access Badges in the Office)**

Policies are like **access badges** in our office analogy. They define **what a user or group is allowed to do** in AWS.

**Example Policies:**

- **AdministratorAccess:** Full control of everything 🚀
- **ReadOnlyAccess:** Can view everything but can’t make changes 👀
- **EC2FullAccess** → Can create, modify, and delete EC2 instances

AWS Policies use JSON (a coding format), but don’t worry—you **don’t need to write code** to apply them. You can use AWS-managed **policies** (pre-made templates) or create custom ones.

1: Go to **AWS IAM → Policies, Create Policy** (or choose an existing one).

2: Select a **user or group** to apply it to.

3: Done! The permissions are now active.

![image.png](image%209.png)

![image.png](image%2010.png)

AWS **Users, Groups, and Policies** are the foundation of **cloud security and access management**. By understanding how they work, you ensure **your AWS environment stays organized, secure, and efficient**.
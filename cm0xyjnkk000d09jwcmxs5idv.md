---
title: "Day 2: Configuring User and Group Accounts in Microsoft Entra ID"
datePublished: Wed Sep 11 2024 14:30:17 GMT+0000 (Coordinated Universal Time)
cuid: cm0xyjnkk000d09jwcmxs5idv
slug: day-2-configuring-user-and-group-accounts-in-microsoft-entra-id
tags: cloud, microsoft, azure, devops, azure-devops, microsoft-azure, azure-certified

---

Welcome to Day 2 of our journey into mastering Azure Identity! Yesterday, we dove deep into **Administering Identity** with an overview of **Microsoft Entra ID**, and its key concepts, and today 2: Configuring User and Group Accounts in Microsoft Entra ID serves as the backbone of Azure's identity and access management. We looked at identity types, authentication methods, and access management, all while keeping security as a top priority.

First, let's start with the Day 1 recap.

### Recap of Day 1

* **Microsoft Entra ID** is the new face of Azure AD, playing the role of a digital gatekeeper for managing access to Azure services.
    
* We explored how **users** and **groups** are central to identity management, working similarly to office building security—allowing only authorized personnel into the right spaces.
    
* Key features like **Hybrid Identity**, **Self-Service Password Reset**, and **Conditional Access** were highlighted as essential tools in keeping the Azure environment both user-friendly and secure.
    

Today, we’ll extend our focus to **Configuring User and Group Accounts**, ensuring each person and service has the right permissions to access the correct resources. Let’s get into it!

---

### Objective 2: Configuring User and Group Accounts in Microsoft Entra ID

Here, we dive into managing identities directly by setting up **user accounts** and **groups** in Microsoft Entra ID. Think of this as issuing digital ID cards and group access to employees, with each cardholder having specific permissions based on their role.

### User Accounts: The Digital ID Cards

A **User Account** in Microsoft Entra ID represents an individual within your organization. User accounts are used for **Authentication** and **Authorization**, ensuring that each individual has a unique identity. Each user account can have roles, permissions, and profile information. Setting up these accounts is like issuing ID cards to employees—each with specific access levels depending on their role.

Administrators have the convenience of accessing all user accounts from a centralized location.

> Microsoft Entra ID --&gt; Users --&gt; All Users

This simplifies the management of user identities across the organization. It also provides the ability to perform Bulk operations.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfrm2a0AIlwu_LJNm0YZWMdRX4c0buUQY7ZepsHu6UlNZ2Hd37OmRuhGh_9HblH_hnca-uK7nhHwtTvaVxI_mPmxsj9hOa80632zeZiOKug5rBl-MBKn-9JoGpCfKCq3OJAReKj6WDBVI6qu2Ab2MWaKH0?key=-AdxUsRmAsOPQMRmmifevQ align="left")

**Real-Life Example: Onboarding a New Employee**

When a new employee joins your company, you don’t just give them the keys to the entire building. You assign them an office, give them access to certain floors, and maybe the break room. Similarly, when you create a new user account in Entra ID, you assign them specific roles and permissions, ensuring they only access the resources they need to perform their job.

User Accounts are of 3 types

\*\*1. Cloud Identities:  
\*\*These exist purely in the cloud, with no ties to on-premises directories. Think of them as digital passports, granting users access from anywhere in the world with ease and agility.

**Example:** A fully remote team member accessing your Azure resources from across the globe would have a cloud identity.

\*\*2. Guest Accounts:  
\*\*Guest accounts are for external users—like partners or contractors—who need specific access without being part of your internal directory.

**Example:** A freelance developer working on a project can access necessary resources through a guest account, without being embedded in your corporate directory.

> **Note:** If the guest is from another company with its own Entra ID, they are still considered a cloud identity. If not, it’s just a personal or non-Entra ID domain account, making it a guest account.

\*\*3. Directory Synchronized Users:  
\*\*These identities are synchronized from an on-premise Active Directory to the cloud using the Microsoft Entra ID Connect tool.

**Example:** An employee who works on-site, with credentials synced from your company’s internal servers to Azure, is a directory-synchronized user.

### **Bulk Operation: Adding tons of Users on one go**

Bulk Operations allows us to download a CSV template where we add users that we want to create, delete, or invite. Using bulk operations, we can easily work on these operations rather than doing them one by one.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeQ8_foEa1QR4zwyneTgyzRWudZxN1Xckc_2zyctSzVcAlr1AD5Av_UcLDPBZVAEFrjHnJEZ4fjD3bh6AJyITAChfOYcx4Je11iaVH4zrKYJ-0bBPTqgOypSPumgqGjTQJUq89tJMHc0vR-wLAEUj6Rl5w1?key=-AdxUsRmAsOPQMRmmifevQ align="left")

**Four Essential Bulk Operations:**

1. **Bulk Create:** Add multiple users at once by uploading a CSV file.
    
    * **Example:** Onboarding a new department—just upload their details, and Entra ID does the rest.
        
2. **Bulk Invite:** Simplify inviting external users.
    
    * **Example:** Inviting all contractors to a specific project at once.
        
3. **Bulk Delete:** Efficiently remove multiple accounts.
    
    * **Example:** Cleaning up after a project ends by deleting all associated contractor accounts.
        
4. **Download Users:** Export user data for reporting or auditing.
    
    * **Example:** Generating a compliance report on user access.
        

### **Groups: Managing Permissions at Scale**

Groups in Microsoft Entra ID allow you to manage permissions for multiple users simultaneously. It’s like having a master key that gives a team access to certain rooms, rather than issuing individual keys for each door.

Imagine you’re managing an IT department. You wouldn’t individually assign access to each server and database to every team member. Instead, you’d create an “IT Team” group in Microsoft Entra ID and assign the necessary permissions to the group. This way, whenever a new member joins the team, you simply add them to the group, and they automatically inherit the group’s permissions.

Group accounts in Microsoft Entra ID are key to managing permissions efficiently.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeGblTNY7ZDNMOJFlFuMMOiochDBdRz6oJhzS9V9ZX01ayUAU5czuomHWsiOkXMZVGXBAAeO_00M7_sOMhyMYSy5lledr9onPv4vZScWc7Gr801OdzWmzbk0oWxCTIqNIFTs9dIM2z1Ym38at4TxIO1IkNi?key=-AdxUsRmAsOPQMRmmifevQ align="left")

**1\. Group Types:**

* **Security Group:** Designed for managing access permissions.
    
    * **Example:** An “Azure Admin” group grants specific users administrative privileges across Azure services.
        
* **Microsoft 365 Groups:** Focused on collaboration, integrating with tools like Outlook and Teams.
    
    * **Example:** A marketing team working on a campaign can share emails, files, and workspaces seamlessly.
        

**2\. Assignment Types:**

* **Assigned:** Members are manually added to the group.
    
    * **Example:** An HR admin adds a new HR associate to the HR resources group.
        
* **Dynamic User:** Automatically adds or removes members based on user attributes.
    
    * **Example:** Any employee with "HR" in their job title is auto-added to the HR group.
        
* **Dynamic Device:** Similar to Dynamic User, but based on device attributes.
    
    * **Example:** Devices running a specific OS are added to a group for targeted software updates.
        

Understanding these group types and assignments ensures that the right people and devices have the right access at the right time.

**Dynamic Groups:** Let’s say you want to automatically add users to a group based on specific attributes, like their department or job title. Dynamic groups in Entra ID can do this for you, automatically updating group membership as user attributes change. It’s like having a security system that updates access permissions as employees change roles.

### **Self-Service Password Reset (SSPR): Empowering Users**

SSPR lets users reset their passwords without needing to call IT, giving them control over their own security. It supports multiple authentication methods like email, phone, or a mobile app, offering layers of protection.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-H5E_1lQ79vr7S5VLbEbMxd6x1GvC0rtvAb-yVkwdAhhe5eFXc4A8hkUiO9uKe919onPST4n4lRXe1j84mQolf6w0FHFbpoMpBZDSuqF1lmzlbFy_vff9KBmlFgs0e39HGSgYPh6qRbEMvjceIXMc-N0k?key=-AdxUsRmAsOPQMRmmifevQ align="left")

**Getting Started with SSPR:**

1. Enable SSPR for all or select users.
    
2. Set the number and type of authentication methods for reset.
    
3. Users will register for SSPR during their next sign-in.
    

**Example:** Imagine an employee forgetting their password over the weekend. With SSPR, they can reset it themselves using their phone, without waiting for Monday morning IT support.

> **Note:** SSPR is a premium feature requiring a Premium P2 license, though admins have access by default.

---

### Wrap-Up for Day 2

Today, we covered the second key objective in administering identity: **configuring user and group accounts**. You’ve now got a strong understanding of how user accounts, groups, and bulk operations work in **Microsoft Entra ID**. With these tools, you’re better equipped to manage identities at scale, ensuring that everyone and every service in your Azure environment has the correct access.

Stay tuned for Day 3, where we’ll begin our deep dive into **Administering Governance and Compliance**—a crucial aspect of keeping your Azure setup secure and compliant.

---

**Hey there! I’m Anurag Raj – your go-to DevOps wizard with a knack for transforming complex operations into seamless, magical CI/CD experiences.**

With 3 years of hands-on expertise in optimizing workflows and boosting productivity, I’m all about turning the ordinary into the extraordinary. Whether it’s crafting innovative solutions or streamlining processes, I bring a touch of magic to everything I do.

Curious about how we can make DevOps even more awesome together? Click the link and drop me a “[**Hello Anurag**](https://www.linkedin.com/in/anurag-raj-8975b0128/)”! Let’s connect and explore the endless possibilities in the world of DevOps.

Excited to chat with you soon!!
---
title: "Day 03: Administer Governance and Compliance"
datePublished: Thu Sep 12 2024 14:30:56 GMT+0000 (Coordinated Universal Time)
cuid: cm0ze0bq9001z08ld0uzq4gkb
slug: day-03-administer-governance-and-compliance
tags: cloud, microsoft, azure, devops, devops-articles

---

Today, we're diving into the fascinating world of **Governance and Compliance** in Azure! Sounds serious, right? Don't worry, we'll keep it light, fun, and informative. Governance in Azure is all about keeping things in order—kind of like being the responsible friend in your group who makes sure nobody loses their phone during a night out. In the cloud, however, it's about making sure your resources and applications are managed and monitored effectively.

Think of compliance as that same friend, but now they're also making sure you follow the rules of the club (or industry standards in this case) to avoid getting into trouble. With that, let’s break down the core learning objectives we’ll be tackling today:

* **Configure Subscriptions and Azure Resource Manager Resources**
    
* **Configure Azure Policies**
    
* **Configure Azure Role-Based Access Control (RBAC)**
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725979192630/71cd6457-ca38-434a-8efa-ee805e6fa583.png align="center")

We'll focus on the first one today, and there's a lot to unpack. So, grab your cloud hat, and let’s dive in! But first, let’s have a recap of Day 2.

### Day 2 Recap: Managing Users and Groups in Microsoft Entra ID

Yesterday, we took a deep dive into Microsoft Entra ID (formerly Azure AD) and learned how to manage user accounts and groups efficiently.

We started by understanding that user accounts in Entra ID are like digital ID cards that represent individuals in your organization. Whether it's a remote worker with a Cloud Identity, a Guest Account for external collaborators, or an on-premises employee with a Directory Synchronized Identity, each user gets unique access based on their role.

We explored Bulk Operations—how to onboard, invite, delete, and even export users with just a CSV file, turning what could be a time-consuming task into a breeze!

Then we jumped into Groups, where managing permissions at scale became a whole lot easier. Imagine having a single key to unlock multiple doors: That’s exactly how groups work. From Security Groups for permission management to Microsoft 365 Groups for seamless collaboration, we discovered the different group types and how Dynamic Groups can automatically update membership based on user attributes—like a self-updating team roster!

Finally, we wrapped up with a game-changer: Self-Service Password Reset (SSPR), which gives users the power to reset their own passwords without bugging IT (because who wants to wait for Monday to fix a locked account?).

With all of this knowledge under our belt, we’re well on our way to mastering identity management in the cloud!

Now that we've wrapped up the summary of Day 2, let's dive into today's topic!

---

### Governance and Compliance: Why Should You Care?

Think of "Governance" as a company’s traffic cop—keeping everything in check, making sure resources are being used effectively, and that no one’s speeding (or overspending). Compliance is your organization’s way of ensuring you follow rules, meet industry standards, and don’t end up with a hefty fine or a chaotic cloud setup!

In Azure, **Governance** is about keeping tabs on what’s happening in your cloud, and **Compliance** helps ensure you meet all those business rules and regulations.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725979242692/274c2e34-c2b6-4d94-a424-bcd4cc89ae02.jpeg align="center")

### Let’s Get Down to Business: **Configure Subscriptions**

Alright, picture this: Subscriptions are like your Netflix account. It’s how you access all your favorite shows (or, in Azure’s case, resources) and manage what you’re subscribed to. If your team is like a household with multiple people sharing the Netflix account, each subscription helps you divvy up the bill while keeping everything organized.

#### Key Features of Azure Subscriptions (Your Cloud Library Card):

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725978912325/3e83c46b-20f8-4845-885a-0d709ca1ec09.png align="center")

1. **Billing Boundary**: Your subscription defines where the bills go—just like your Netflix subscription tells you how much you owe every month for binge-watching shows.
    
2. **Resource Organization**: All your cloud goodies (VMs, storage, databases) live under a subscription. Think of it as your personalized library of cloud services.
    
3. **Environment Boundaries**: Subscriptions can help you separate projects. Need one for development and one for production? No problem. Separate them, just like organizing your bookshelves.
    
4. **Subscription ID**: It’s like your library card number, ensuring every cloud resource or transaction can be tracked back to you.
    
5. **Multiple Subscriptions?**: Yup! You can have several, just like how you might have separate Spotify and Netflix accounts—one for work, one for play.
    

### **Subscription Types (Your Ticket to the Cloud)**

Azure’s got options. Whether you're a solo developer or running a huge enterprise, there’s a subscription type for you!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725979122226/69a69c29-d6a4-4be3-8fc3-8fc053851bb8.png align="center")

1. **Enterprise Agreements**: Like bulk-buying popcorn for a movie marathon, these subscriptions are great for large organizations. You commit to using a certain amount of cloud resources (say, 1 million dollars worth) and get a better rate.
    
    *Real-world example*: A big company like Contoso, with hundreds of developers, signs an Enterprise Agreement to manage all their cloud projects under one roof, with the promise that they’ll use a certain amount of resources each year.
    
2. **Pay-As-You-Go**: Just like ordering pizza on the fly—you only pay for what you consume! Perfect for companies that don’t want long-term commitments.
    
    *Real-world example*: A startup uses the Pay-As-You-Go option for their testing environment, where they can scale up or down depending on how much testing they’re doing that month.
    
3. **Cloud Solution Provider (CSP)**: Imagine having a cloud expert buddy who helps you set everything up. CSPs allow businesses to partner with experts who tailor cloud solutions for them.
    
    *Real-world example*: Your company outsources its Azure subscription to a CSP to get better rates and specialized support for Azure services.
    
4. **Free Trial**: Want to test the waters without getting wet? The Free Trial subscription lets you explore Azure without any upfront costs. You get a limited amount of credits, and when they're gone, your subscription turns into a pumpkin (or, more realistically, a Pay-As-You-Go plan).
    
5. **Azure for Students**: Who doesn’t love free stuff? Students get free access to Azure, along with some credits to play around with.
    
6. **Visual Studio Subscription**: This one’s a developer’s dream. Visual Studio users get access to Azure resources and tools, making development and testing a breeze.
    

Subscriptions act like the backbone of your Azure environment, helping you manage everything from billing to resource organization. Whether you’re running a multinational company or experimenting with the cloud for the first time, there’s a subscription plan tailored just for you. Just like choosing the right Netflix plan, it’s all about picking the one that suits your needs.

---

### Up Next on Day 4...

In Day 4, we’ll continue our journey into **Azure Resource Manager** and tackle **Resource Groups and Limits**. Think of Resource Groups as your cloud filing system—where you organize resources into neat folders. It’s going to be a blast (and super useful)!

So, buckle up because we’re going to make managing cloud resources feel as simple as organizing your bookshelf! Keep learning, keep growing, and let’s conquer Azure one day at a time.
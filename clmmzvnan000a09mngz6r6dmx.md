---
title: "Luscious Linux"
seoTitle: "Linux, Linux for DevOps, Linux Command"
datePublished: Sun Sep 17 2023 05:06:16 GMT+0000 (Coordinated Universal Time)
cuid: clmmzvnan000a09mngz6r6dmx
slug: luscious-linux
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/4Mw7nkQDByk/upload/7bcf1ebbaa28345c3fbb0ca5a49ea855.jpeg
tags: linux, devops, linux-for-beginners, devops-articles, devopscommunity

---

If you are in the initial phase of your professional life or you are a student in a college, you might have heard the term "Linux". Most of the seniors you are interacting with must have suggested learning Linux. But what is Linux and why is it important? In this blog, we are going to explore the world of Linux from a beginner perspective. So, let's get started.

## History of Linux

In the year 1991, a student of the University of Helsinki, Finland, USA, Linus Torvalds, developed an open-source operating system known as Linux. Since then, years have passed and it's become the most popular operating system.

At that time, when Linux was not developed, most operating systems were proprietary and expensive. Linus Torvalds aimed to develop an operating system that would be freely accessible to all users. Initially, he introduced Linux as open-source software, distributed under the GNU General Public License. Consequently, this allowed anyone the freedom to utilize, modify, and share his source code without any restrictions.

Linux is like a superhero among computer operating systems. It's super stable, ultra-secure, and incredibly reliable. People use it a lot in places where they need their computers to be rock-solid, like big servers, super-powerful supercomputers, and serious business environments.

Linux is such a big deal that it's practically everywhere! Around 2.76% of regular computers use it as their main system, but that number jumps way up when you look at supercomputers – over 90% of the world's most powerful ones run on Linux. And here's a fun fact: about 71.85% of all those cool smartphones and tablets out there are powered by Android, which is based on Linux. So, in a way, Linux is like the secret sauce that makes a lot of our tech work smoothly!

Linux is a versatile operating system that excels in supporting multiple users and running several tasks simultaneously. It offers a robust command-line interface called the shell, which empowers users with powerful control over their systems. It comes in various flavors or distributions, catering to different preferences and needs.

Flavors are nothing but the type of Linux OS just like we have in Microsoft, for example, XP, Vista, Windows 7, 10, and 11. Similarly, in Linux, there are various flavors available and a few of them are:

* Ubuntu
    
* Fedora
    
* Debian
    
* Linux Mint
    
* Solaris
    
* openSUSE
    
* CentOS and many more.
    

> Fun Fact: Linux provides the updates twice in a year and that to in April and October.

## Architecture of Linux

Before building a new house, it is important to understand its architecture. The same is applicable here as well. Before proceeding ahead, it is important for us to understand the architecture of Linux and how Linux works.

Understanding the architecture of Linux is like peering behind the curtain of a magical performance. It's a blend of meticulous organization, efficient communication, and powerful components that work together to create a stable and versatile operating system.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694921121600/b07df6f2-fcca-484e-9ca8-25fd94369b7c.jpeg align="center")

### 1\. Kernel Layer: The Core Engine

Imagine the Linux kernel as the engine of a car. It's the heart of the operating system, responsible for managing hardware resources like your CPU, memory, and devices. When your computer boots up, the kernel is the first thing that springs into action, making sure everything runs smoothly. It's like the conductor of a grand orchestra, coordinating all the instruments.

> Fun Fact: The Kernel of Linux Operating System is also called Linux

### 2\. Shell Layer: The Command Interpreter

Now, let's talk about the shell. Think of it as the language you use to communicate with your Linux system. Just like you speak English or any other language, you communicate with Linux using commands. The shell takes your commands and translates them into actions that the kernel understands. It's like a personal assistant that carries out your instructions.

3\. User Space/Applications: Where You Live and Work

The user space is where you spend most of your time. It's where your applications and programs run. This is where you write documents, browse the web, and do all your day-to-day tasks. It's like your office or your home - the place where you get things done.

### How These Layers Interact

Imagine a pyramid, with the kernel at the base, the shell above it, and the user space applications at the top. When you type a command (e.g., "ls" to list files), it starts at the top (user space). The shell understands it and sends the request down to the kernel. The kernel then performs the requested action and sends the results back up to the shell, which finally displays the information to you.

Linux's architecture is like a Lego set for your computer. You can build your own unique system by choosing different components, just like you can build amazing structures with Lego bricks. You can customize it to suit your needs, making it incredibly versatile.

## File System Hierarchy

In the world of Linux, there's a fascinating concept that sets it apart from other operating systems: the idea that everything, from your text documents to your computer's hardware, is represented as a file. It's like a giant digital filing cabinet, organized in a tree-like structure. Let's explore this concept, known as the "Linux File System Hierarchy,"

**The Tree-Like Structure:** Think of your Linux system as a tree, with the trunk representing the root directory, often denoted as '/'. This root directory is the starting point for everything on your computer. Just like a tree's branches, the root directory has many subdirectories, and these subdirectories can have more subdirectories of their own. It's a hierarchical structure, much like the folders on your desk, but on a grand scale.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694926204583/1ec957e1-5b56-4037-abf4-9706febefca6.png align="center")

**Files and Directories:** In this digital filing cabinet, everything is either a file or a directory. Files can hold all sorts of data, like your music, photos, or even the programs that run your computer. Directories, on the other hand, are like folders that help you organize your files. They can contain files or even more directories.

**Hardware as Files:** One fascinating aspect of Linux is how it treats hardware. In Linux, even your computer's hardware components, like the keyboard, mouse, or display, are represented as files! This unique approach allows Linux to interact with hardware in a consistent and predictable way.

**Examples:**

* Your text document is a file.
    
* The music you play is stored in files.
    
* When you plug in a USB drive, it appears as a file.
    
* Your computer's CPU is represented as a file.
    

**Why Does It Matter?** Understanding this file-centric approach is crucial, especially for those exploring Linux for the first time. It simplifies how you interact with your computer, whether you're creating, moving, or deleting files. It also lays the foundation for powerful automation and scripting possibilities in Linux.

## User Account on Linux

User accounts are like personalized keys to your computer kingdom. They allow you to have your own space, settings, and permissions on a Linux system. Whether you're a beginner or an IT pro, grasping the concept of user accounts is fundamental. Let's explore this in both a professional and beginner-friendly way.

**User Accounts - The Basics:** At its core, a user account in Linux is like having your own room in a big house. It's where you store your files, set your preferences, and do your work. But just like in a shared house, you have to follow some rules. These rules are your permissions, and they determine what you can and can't do on the system.

**Types of User Accounts:** Linux typically has two main types of user accounts:

1. **Regular User Accounts:** These are for everyday use. When you log in with a regular account, you can work on your own stuff, but you can't mess with important system files or settings. It's like having a room in the house where you can decorate it as you like, but you can't change the structure of the house.
    
2. **Root User Account:** This is the master key to the house. The root user can do anything, change anything, and access everything. However, with great power comes great responsibility. It's crucial to use the root account carefully because you can accidentally break things if you're not cautious.
    

**User Account Management:** Managing user accounts on Linux involves tasks like creating, deleting, and modifying them. These actions are typically carried out by a superuser or administrator, who has the power to make changes for all users. It's like having a building manager who can assign rooms and manage the house rules.

User accounts are vital for security and organization. They ensure that different users can't accidentally (or intentionally) interfere with each other's work. They also help protect the system from unauthorized access.

## Linux & DevOps

Linux plays a pivotal role in the world of DevOps for several key reasons:

1. **Open Source Philosophy:** Linux is open-source software, which means its source code is freely available for anyone to view, modify, and distribute. This aligns with the principles of DevOps, fostering collaboration, transparency, and community-driven innovation.
    
2. **Stability and Reliability:** Linux is known for its robustness and stability. In DevOps, where continuous integration and continuous delivery (CI/CD) pipelines are crucial, a stable operating system is essential to ensure consistent and reliable automation processes.
    
3. **Customization and Flexibility:** Linux offers a high degree of customization. DevOps teams can tailor Linux distributions to suit their specific requirements and workloads. This flexibility allows for the creation of highly optimized and efficient environments.
    
4. **Scripting and Automation:** Linux provides a powerful command-line interface and scripting capabilities through shells like Bash. DevOps heavily relies on automation, and Linux's scripting capabilities enable the automation of repetitive tasks, making it a preferred choice for DevOps practitioners.
    
5. **Containerization and Orchestration:** Linux is at the core of containerization technologies like Docker and container orchestration platforms like Kubernetes. These technologies are fundamental to DevOps for packaging, deploying, and managing applications consistently across different environments.
    
6. **Cloud Compatibility:** Most major cloud providers, including Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP), offer Linux-based virtual machines and container services. Linux's ubiquity ensures seamless integration with cloud-based DevOps practices.
    
7. **Security and Scalability:** Linux distributions are known for their strong security features and the ability to scale horizontally by adding more servers or containers as needed. In DevOps, this is critical for managing infrastructure efficiently and securely.
    
8. **Cost-Efficiency:** Linux is cost-effective since it's open source and doesn't involve licensing fees. This cost savings is appealing to many organizations, especially startups and small businesses adopting DevOps practices.
    
9. **Community and Support:** Linux has a vast and active user community, along with comprehensive documentation and online resources. DevOps practitioners can readily find help, troubleshoot issues, and learn from others in the Linux community.
    
10. **Compatibility with DevOps Tools:** Many DevOps tools and technologies, such as Ansible, Jenkins, Terraform, and Git, have strong support for Linux platforms. These tools are essential for automating infrastructure provisioning, continuous integration, and deployment pipelines.
    

In summary, Linux is the backbone of many DevOps practices, providing a solid foundation for automation, scalability, and customization. Its open-source nature, stability, and compatibility with DevOps tools make it an indispensable choice for DevOps professionals aiming to streamline and accelerate software development and delivery processes.

## Some Important Commands

Linux is nothing without the commands. For every task you have to write a command, so below are some of the Important commands which you'll probably use in your routine.

### Help

| Command | Description | Why The Name |
| --- | --- | --- |
| [man](https://www.tutorialworks.com/linux-commands/#man) | Show help (the manual) | manual |
| [which](https://www.tutorialworks.com/linux-commands/#which) | Find out where a command is | which location? |
| [\--help](https://www.tutorialworks.com/linux-commands/#command-help) | Find help on any command | help! |
| [Ctrl+C](https://www.tutorialworks.com/linux-commands/#ctrl-c) | Stop the current program |  |
| [:q!](https://www.tutorialworks.com/linux-commands/#q) | Quit the *vi* text editor without saving | quit! |

### Logging in and out

| Command | Description | Why The Name |
| --- | --- | --- |
| [logout](https://www.tutorialworks.com/linux-commands/#logout) | Exit the current login shell |  |
| [passwd](https://www.tutorialworks.com/linux-commands/#passwd) | Change your password | password |
| [sudo](https://www.tutorialworks.com/linux-commands/#sudo) | Execute a command as a superuser | super-user do |
| [ssh](https://www.tutorialworks.com/linux-commands/#ssh) | Create an SSH connection (a terminal) to a server | secure shell |

### Moving around the file system

| Command | Description | Why The Name |
| --- | --- | --- |
| [cd](https://www.tutorialworks.com/linux-commands/#cd) | Change the current directory (folder) | change directory |
| [ls](https://www.tutorialworks.com/linux-commands/#ls) | List files in a directory | list |
| [mkdir](https://www.tutorialworks.com/linux-commands/#mkdir) | Make/create a new directory | make directory |
| [pwd](https://www.tutorialworks.com/linux-commands/#pwd) | Print current directory | print working directory |
| [cp](https://www.tutorialworks.com/linux-commands/#cp) | Copy files and directories | copy |
| [rm](https://www.tutorialworks.com/linux-commands/#rm) | Delete files and directories | remove |

### Find, view, and edit files

| Command | Description | Why The Name |
| --- | --- | --- |
| \[cat\](https://www.tutorialworks.com/linux-commands/#cat) | Print the contents of a file | concatenate |
| [chmod](https://www.tutorialworks.com/linux-commands/#chmod) | Change the permissions of a file or directory | change mode |
| [chown](https://www.tutorialworks.com/linux-commands/#chown) | Change the owner and group of a file or directory | change owner |
| [diff](https://www.tutorialworks.com/linux-commands/#diff) | Show the difference between the two files | difference |
| [file](https://www.tutorialworks.com/linux-commands/#file) | Show the type of file |  |
| [less](https://www.tutorialworks.com/linux-commands/#less) | Browse the contents of a file | opposite of 'more' |
| [locate](https://www.tutorialworks.com/linux-commands/#locate) | Find files with names matching a pattern |  |
| [tail](https://www.tutorialworks.com/linux-commands/#tail) | Print the last few lines of a file | tail end (of something) |
| [touch](https://www.tutorialworks.com/linux-commands/#touch) | Create a new file or update an existing one |  |
| [nano](https://www.tutorialworks.com/linux-commands/#nano) | An interactive file editor | Nano's ANOther Editor |
| [vim](https://www.tutorialworks.com/linux-commands/#vim) | An interactive file editor (Intermediate level) | visual improved |

And that's it for today's learning. Happy learning 🧡

---

Hi there, I am Anurag Raj, an Experienced DevOps Engineer with 2.7 Years of Expertise in Streamlining Operations, Enhancing Efficiency, and Enabling Continuous Integration and Deployment.

You can say Hey to me by clicking the below link.

[Hello Anurag](https://www.linkedin.com/in/anurag-raj-8975b0128/) 🧡

If you liked this article, consider sharing it.

#devops #linux
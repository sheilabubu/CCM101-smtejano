# Laboratory 01 – Welcome to the Cloud

## Mission Overview

This laboratory activity introduced us to the fundamentals of cloud computing and Linux-based environments. We used the KillerCoda Ubuntu Playground to perform basic tasks in a Linux terminal and created a GitHub repository as our Cloud Computing Portfolio. Through the different activities, we practiced using Linux commands, checking system details, managing users, organizing files and directories, and creating technical documentation using Markdown.

## Objectives

* Learn how to access and operate a Linux environment through KillerCoda.
* Create and configure a Linux user account.
* Use basic commands to explore the Linux operating system.
* Check important system information and resources.
* Create, organize, and manage files and directories.
* Set up a public GitHub repository for laboratory outputs.
* Develop proper technical documentation using Markdown.

## Activities Performed

For this laboratory, we started an Ubuntu 24.04 environment through KillerCoda and tested the terminal to make sure it was functioning correctly. We created the Linux user account `smtejano`, set a password, and gave the account sudo access. After switching to the newly created account, we used different commands to examine the operating system, kernel, CPU, memory, and disk storage. We also created several directories to organize our laboratory files and made a Markdown file for documentation. Lastly, we created and organized our GitHub repository named `CCM101-smtejano`, which was used to store our laboratory activities, screenshots, and other required outputs.

## Linux Commands Used

The following commands were used to complete the laboratory tasks:

```bash
whoami
pwd
hostname
useradd -m -s /bin/bash smtejano
passwd smtejano
usermod -aG sudo smtejano
su - smtejano
cat /etc/os-release
uname -r
lscpu | grep "Model name"
free -h
df -h /
mkdir Documents Notes Reports Screenshots
ls
cd Notes
pwd
nano about-me.md
cat about-me.md
```

## Skills Learned

This laboratory helped me understand the basic operations of a Linux environment and how it can be used in cloud computing. I learned how to create a Linux user, assign permissions, switch between user accounts, and use commands for navigating and managing files. I also learned how to obtain system information, including the operating system version, kernel, CPU, memory, and storage capacity. Furthermore, I gained practical experience in creating a GitHub repository and using Markdown to document my laboratory work. These skills provided me with a better foundation for completing more advanced cloud computing activities in the future.

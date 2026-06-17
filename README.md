# Active Directory User Management Lab

## Project Overview

This project is a hands-on Active Directory home lab built with Windows Server 2025, Windows 11 Enterprise Evaluation, and Oracle VirtualBox.

The goal of this lab was to practice common Tier 1 help desk and IT support tasks in a Windows domain environment. The lab includes creating a domain controller, configuring a domain, creating Organizational Units, managing user accounts, resetting passwords, creating security groups, disabling accounts, and joining a Windows client computer to the domain.

## Lab Environment

* **Virtualization:** Oracle VirtualBox
* **Server OS:** Windows Server 2025 Standard Evaluation
* **Client OS:** Windows 11 Enterprise Evaluation
* **Domain:** johnlab.local
* **Domain Controller:** AD-SERVER
* **Client Computer:** AD-CLIENT
* **Server IP Address:** 192.168.10.10
* **Client IP Address:** 192.168.10.20

## Skills Demonstrated

* Windows Server installation and setup
* Active Directory Domain Services installation
* Domain Controller promotion
* DNS configuration for domain communication
* Organizational Unit creation
* User account creation
* Password reset workflow
* Account disable and enable workflow
* Security group creation
* Adding users to security groups
* Moving users between Organizational Units
* Joining a Windows 11 client to an Active Directory domain
* Verifying domain user login with Command Prompt
* IT documentation and screenshot-based reporting

## Lab Steps Completed

### 1. Installed Windows Server

Installed Windows Server 2025 Standard Evaluation in VirtualBox and verified access to Server Manager.

### 2. Renamed the Server

Renamed the server to `AD-SERVER` to clearly identify it as the domain controller.

### 3. Installed Active Directory Domain Services

Installed the Active Directory Domain Services role from Server Manager.

### 4. Promoted Server to Domain Controller

Promoted the server to a domain controller and created a new forest using the domain:

```text
johnlab.local
```

### 5. Created Organizational Units

Created the following Organizational Units:

* Employees
* IT
* Sales
* Disabled Users

### 6. Created User Accounts

Created test domain users:

* Jordan Smith
* Maria Garcia

### 7. Performed Password Reset

Reset the password for Jordan Smith and required the user to change the password at next logon.

### 8. Created Security Group

Created a security group named:

```text
IT Support
```

### 9. Added User to Security Group

Added Jordan Smith to the IT Support security group.

### 10. Disabled and Organized User Account

Disabled Jordan Smith’s account and moved it into the Disabled Users OU to simulate a common offboarding or account cleanup task.

### 11. Configured Client Networking

Configured the Windows 11 client with a static IP address and pointed DNS to the domain controller.

### 12. Joined Windows 11 Client to Domain

Joined the Windows 11 client computer to the `johnlab.local` domain.

### 13. Verified Domain User Login

Logged in successfully as the domain user:

```text
johnlab\mgarcia
```

Verified the login using Command Prompt:

```cmd
whoami
hostname
```

## Screenshots

Screenshots are included in the `/screenshots` folder and document each major step of the lab, including server setup, Active Directory configuration, user management, password reset, group membership, domain join, and domain user verification.

## What I Learned

Through this project, I practiced real-world help desk and Windows administration tasks that are commonly used in IT support environments. I gained hands-on experience with Active Directory, user account management, password resets, security groups, Organizational Units, DNS-based domain communication, and joining a Windows client to a domain.

This lab helped me better understand how companies manage users, computers, permissions, and authentication in a Windows domain environment.

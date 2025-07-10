osTicket – Prerequisites and Installation
<p align="center"> <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/> </p>
Overview
This guide walks through the prerequisite setup and installation process for the osTicket open-source support ticket system. It’s intended to be deployed in a Windows environment using Microsoft Azure, IIS, and PHP/MySQL stack.

🧰 Environments and Technologies Used
Microsoft Azure – Virtual Machines / Compute

Remote Desktop Protocol (RDP)

Internet Information Services (IIS) – Used to host the osTicket web application

🖥️ Operating System Used
Windows 10 (21H2)

✅ List of Prerequisites
Before installing osTicket, make sure the following components are installed and configured:

IIS (Internet Information Services) – Web server

PHP (v7.3–v8.1) – Scripting language required by osTicket

MySQL (or MariaDB) – Database backend

osTicket Installation Files – Downloaded from osTicket's official website

Required IIS Features – Such as CGI, PHP handler, and URL Rewrite Module

<p align="center"> <img src="https://github.com/user-attachments/assets/61d5ffbe-bb34-4c71-905e-e629dd277336" width="80%" alt="Windows Features Required for osTicket"/> </p>
Screenshot: Windows features enabled for IIS and osTicket compatibility.

🔧 Installation Steps
1️⃣ Install IIS and PHP

![image](https://github.com/user-attachments/assets/30047273-92a9-4edf-909b-3df6e7042f2a)


Install IIS through "Turn Windows features on or off", and verify PHP is installed and configured correctly using phpinfo().

2️⃣ Download and Extract osTicket

![image](https://github.com/user-attachments/assets/26eb1120-57d5-43fb-9fd3-a4a5e2203401)


Download osTicket from the official site, extract files into C:\inetpub\wwwroot\osticket, and configure permissions.

3️⃣ Create MySQL Database for osTicket

![image](https://github.com/user-attachments/assets/83c2a02c-e15c-4a58-b8a3-6f4b1200d29e)

Using MySQL Workbench or command-line, create a database and user with appropriate permissions for osTicket.

4️⃣ Run osTicket Web Installer

![image](https://github.com/user-attachments/assets/60c477bc-25b7-4d8f-a9c2-b74bb2e97c9e)

Navigate to http://localhost/osticket/setup in your browser and complete the installer with your database and admin details.

✅ Summary
This guide covers:

Installation of IIS, PHP, and MySQL on a Windows 10 VM

Deployment of osTicket via IIS

Configuration of prerequisites for a functional help desk system

osTicket is now ready for post-installation configuration, including department setup, email integration, and ticket workflow customization.

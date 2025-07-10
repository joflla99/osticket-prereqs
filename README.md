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
<p align="center"> <img src="https://i.imgur.com/DJmEXEB.png" width="80%" alt="IIS Installation"/> </p>
Install IIS through "Turn Windows features on or off", and verify PHP is installed and configured correctly using phpinfo().

2️⃣ Download and Extract osTicket
<p align="center"> <img src="https://i.imgur.com/DJmEXEB.png" width="80%" alt="osTicket Setup Files"/> </p>
Download osTicket from the official site, extract files into C:\inetpub\wwwroot\osticket, and configure permissions.

3️⃣ Create MySQL Database for osTicket
<p align="center"> <img src="https://i.imgur.com/DJmEXEB.png" width="80%" alt="MySQL Setup"/> </p>
Using MySQL Workbench or command-line, create a database and user with appropriate permissions for osTicket.

4️⃣ Run osTicket Web Installer
<p align="center"> <img src="https://i.imgur.com/DJmEXEB.png" width="80%" alt="Web Installer"/> </p>
Navigate to http://localhost/osticket/setup in your browser and complete the installer with your database and admin details.

✅ Summary
This guide covers:

Installation of IIS, PHP, and MySQL on a Windows 10 VM

Deployment of osTicket via IIS

Configuration of prerequisites for a functional help desk system

osTicket is now ready for post-installation configuration, including department setup, email integration, and ticket workflow customization.

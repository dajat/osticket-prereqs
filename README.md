<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create Virtual Machine in Microsoft Azure
- Install/Enable Internet Information Services (IIS) in Windows with CGI and download PHP Manager for IIS
- Download and Install Rewrite Module and Create directory for PHP to unzip files
- Download and Intsall VC file and MySQL
- Register PHP in IIS and reload to install osTicket v1.15.8
- Enable required extensions to continue installation of osTicket
- Install HeidiSQL to link MySQL database to osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create virtual machine in Microsoft Azure and ensure that the OS is Windows 10 with at least 4 virtual CPUs.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install and enable IIS in Windows with CGI. Ensure to download appropiate files and setup configuration as required.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Rewrite module and unzip files for PHP folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install and download VC file and MySQL. Ensure that MySQL is installed in Typical Setup and Launch Confifuration Wizard (after install). Next, install as a Standardd Configuration and add password.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an administrator and register PHP within IIS. Reload IIS (Stop and Start the Server) and install osTicket v1.15.8.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS (Stop and Start the Server) and enabled required extensions (IIS, sites -> Default -> osTicket. Rename: ost-config.php and assign permissions in ost-config.php. Continue to setup osTicket in the browser
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install HeidiSQL, create password and name database. Continue setting up osTicket in the browser
</p>
<br />

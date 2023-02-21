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

<h2>Step 1: Create a Virtual Machine in Microsoft Azure</h2>
<p>
<img src="https://i.imgur.com/TT8okiI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create virtual machine in Microsoft Azure and ensure that the OS is Windows 10 with at least 4 virtual CPUs.
</p>
<br />

<h2>Step 2: Install and Enable Internet Information Services (IIS) in Windows with CGI </h2>
<p>
<img src="https://i.imgur.com/34jHtDx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create virtual machine in Microsoft Azure and ensure that the OS is Windows 10 with at least 4 virtual CPUs. Once you have logged into the remote desktop connection, go to the control panel, select Programs and Turn on or off Windows features and select the following to enable IIS with CGI on Windows 10.
</p>
<br />

<h2>Step 3: Download and Install PHP Manager for IIS, Rewrite Module, and create the directory C:\PHP</h2>
<p>
<img src="https://i.imgur.com/7kEgub5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and Install PHP Manager for IIS to run osTicket on the web browser. Also, download and Install the Rewrite Module and create a PHP folder in the windows directory.
</p>
<br />

<h2>Step 4: Download and unzip PHP 7.3.8 in PHP folder </h2>
<p>
<img src="https://i.imgur.com/U8k2kuk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and extract all PHP files in to the previously created PHP folder.
</p>
<br />

<h2>Step 5: Download and install VC_redist and MySQL </h2>
<p>
<img src="https://i.imgur.com/EbyvS5F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install Microsoft Visual C++ and MYSQL. Ensure that MySQL is downloaded for "Typical Setup" and Launch Configuration Wizard (after insall) is checked. Continue to install as Standard Configuration and add a password for MySQL.
</p>
<br />

<h2>Step 6: Open IIS as an Admin and Register PHP in IIS </h2>
<p>
<img src="https://i.imgur.com/KdMo93q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Run IIS as an Administrator and register PHP in IIS. Once PHP has been registered make sure to restart the server.
</p>
<br />

<h2>Step 7: Reload IIS and Install osTicket </h2>
<p>
<img src="https://i.imgur.com/TT8okiI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After restarting the server, Install that osTicket file from the installation folder. Extract and copy the "upload folder" to c:\inetpub\wwwroot
</p>
<br />

<h2>Step 8: Reload IIS and Browse to *:80 to review what extensions need to be enabled </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to sites, default, osTicket and click on "Browse *:80" to open osTicket in a web browser
</p>
<br />

<h2>Step 9: Enabled extensions in IIS </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to IIS, sites, Defualt, osTicket, double click PHP Manager, click on Enable or disable an extension. Enable the following extensions and observe the changes in the osTicket site on the web browser
</p>
<br />

<h2>Step 10: Rename: ost-config in PHP folder </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Remove sample from "ost-sampleconfig.php by following C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
</p>
<br />

<h2>Step 11: Assign Permissions in ost-config.php and continue to setup osTicket </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to ost-config.php, right click, select properties, select security, and select advanced. Click on everyone, click on edit, and change to only read and read and view
</p>
<br />

<h2>Step 12: Download and install HeidiSQL and contiue to setup osTicket in the browser </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install HeidiSQL. Add in password from MySQL setup to connect the database.
</p>
<br />

<h2>Step 13: Delete "setup" folder in osTicket file and Set permissions to Read only in ost-config.php </h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Delete setup folder in osTicket and change permissions in ost-config.php
</p>
<br />

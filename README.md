#<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Instal and Enable IIS (Internet Information Services) with CGI
- Install PHP for IIS using PHP Manager (5.6 or higher)
- Install MySQL Database
- Install and Rewite Module for IIS
- Download and Configure osTicket Files

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/e78c9d3d-1496-424a-b948-a96cda719e83)

Installing and Configuring Web Server (IIS) and PHP
  - Install IIS and enable the CGI feature under the "Application Development Features" section.
  - Install PHP Manager for IIS and the Rewrite Module
  - Download PHP 7.3.8 and extract it to C:\PHP
  - Install necessary dependencies, including VC_redist.x86.exe and MySQL (version 5.5.62), and
 configure MySQL with the root username and password (root).
  
<br />

![image](https://github.com/user-attachments/assets/0370ca27-17fa-4f57-8ca5-aa3672681e1a)

Setting Up osTicket Files and Configurations
- Download and unzip the osTicket installation files and copy the "upload" folder to C:\inetpub\wwwroot.
- Rename the "upload" folder to "osTicket" and configure IIS to serve the osTicket site.
- Enable PHP extensions like php_imap.dll, php_intl.dll, and php_opcache.dll via PHP Manager in IIS.
- Rename the configuration file from ost-sampleconfig.php to ost-config.php and set the correct file permissions
<br />

![image](https://github.com/user-attachments/assets/c6a6bed3-81e0-4e7c-84fc-d832e265c203)

Completing osTicket Installation
- Create the MySQL database (osTicket) using HeidiSQL.
- Finish the osTicket setup through the browser by entering MySQL database credentials and clicking "Install Now!"
- Access the helpdesk by browsing to http://localhost/osTicket/scp/login.php for admin login and http://localhost/osTicket/ for end users.
</p>
<br />

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

- Microsoft Azure (VM)
- Remote Desktop Access
- Internet Information Services (IIS)
- MySQL Database Server
- PHP
- Web Browser (Google Chrome, Microsoft Edge, Mozilla Firefox)

<h2>Installation Steps</h2>

<p>
![image](https://github.com/user-attachments/assets/09501009-bce6-49d4-9600-3968060277b1)

</p>
<p>
Download and Prepare Files
  
Begin by downloading the latest stable release of osTicket from the official website. Once downloaded, upload the extracted files to the IIS web server’s root directory (C:\inetpub\wwwroot\osTicket). You can use Remote Desktop to access the Azure VM and manage file uploads. Make sure the files are properly extracted and placed in the correct directory for IIS to access.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure IIS and PHP

In IIS, set up a new website or application pointing to the osTicket folder you just uploaded. Ensure that PHP is installed and configured correctly in IIS, including necessary extensions like GD, MySQLi, and MBstring. You may need to configure PHP settings (e.g., php.ini) for optimal performance with osTicket. Also, verify that the necessary permissions are set for the include, attachments, and scripts folders.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set Up MySQL Database and Run Installer

Create a new MySQL database and user for osTicket using MySQL Workbench or the MySQL command line. After configuring the database, open a browser on your local machine and navigate to http://your-vm-ip/osTicket. The osTicket installation wizard will guide you through the remaining steps, including database connection setup. Complete the installation by following the prompts, and be sure to delete the setup directory for security once the process is finished.
</p>
<br />

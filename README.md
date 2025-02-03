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

    1. Set Up IIS and Install Dependencies

Enable IIS with CGI on Windows through the Windows Features menu. Install PHP Manager for IIS and the IIS Rewrite Module from the osTicket installation files. Create a C:\PHP directory and extract PHP 7.3.8 into it. Finally, install the Microsoft Visual C++ Redistributable to support PHP.

    2.  Install MySQL and Configure IIS

Install MySQL 5.5.62 and select the Standard Configuration during setup. Set the root username and password. Open IIS Manager, navigate to PHP Manager, and register PHP by pointing it to C:\PHP\php-cgi.exe. Restart IIS to apply the changes.

    3.  Install and Configure osTicket

Download and extract osTicket v1.15.8, then move the upload folder to C:\inetpub\wwwroot. Rename it to osTicket to ensure proper functionality. Restart IIS, then open a web browser and navigate to http://localhost/osTicket to begin the installation process.

    4.  Adjust Configuration and Set Permissions

Locate the file ost-sampleconfig.php inside C:\inetpub\wwwroot\osTicket\include and rename it to ost-config.php. Open the file properties, disable inheritance, remove all existing permissions, and grant full control to Everyone. Restart IIS once again to ensure the changes take effect.

    5.  Set Up the Database and Finalize Installation

Install HeidiSQL, open it, and create a new session using login credentials. Within the session, create a database named osTicket. Return to the osTicket setup page in the browser, enter the database details, and click "Install Now!" Once the installation is complete, your osTicket help desk system should be fully operational.

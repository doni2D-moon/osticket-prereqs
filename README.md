<p align="center">
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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/988cb74c-ca57-4646-9df8-99d24f134bff)

<p>
1) Open the Control Panel and go to Uninstall Programs 2) Click Turn Windows features on or off 3) Locate "Internet Information Services" and check it. 4)Then check "CGI" under "WorldWide Web Services" and "Application Development Features"
</p>
<br />

![image](https://github.com/user-attachments/assets/77f11d8d-1390-4d7f-a177-a2266fb2d80e)

<p>
After installing the PHP Manager for IIS and the Rewrite Module, 1) Right-click on the PHP file to extract 2)Click on "Browse" to look for the PHP folder in Windows C:\ 3)Click the folder and extract files in the PHP folder.
</p>
<br />

![image](https://github.com/user-attachments/assets/b0496faf-11f2-49e1-a29e-9e44a6925317)

<p>
After installing VC redist, 1) install MySQL 2) During installation, type in a password that will be needed in the setting up osTicket browser page (this can be found at the bottom of the setup page that reads "My SQL Database" along with the username and password 3) Then click "Next" to finish the installation.
</p>
<br />

![image](https://github.com/user-attachments/assets/c581c291-269f-4353-856e-8a7d3ea4bd28)

<p>
After installing osTicket, moving the "upload" file to c: inetpubwwwroot, renaming it to "osTicket," and reloading IIS, 1) Open IIS as admin (that was already done to register PHP and reload) and click on Sites --> Default Web Site --> osTicket 2) On the far right, click "Browse *:80 (HTTP)" 3) A page called "osTicket Installer" will load up in the browser, with prerequisites and recommendations on the page.
</p>
<br />

![image](https://github.com/user-attachments/assets/dd968e6f-d71f-456f-905e-2c3c7fc76867)

<p>
For it to work properly, 3 extensions will need to be enabled. After clicking on PHP shown with other applications in the middle of IIS and clicking on enable/disable PHP extensions on the bottom, 1) Locate php_imap.dll and php_intl.dll with other extensions that are grayed below and enabled them, they will show up in black when enabled 2) Locate the php_opcache.dll with "Disabled" next to it 3) Click on it or go to the right to "Enable". After enabling the extensions, reloading the osTicket Installer page will show two "Recommended" enabled.
</p>
<br />

![image](https://github.com/user-attachments/assets/c9cffc66-4f1f-406e-a9c1-db1029238287)

<p>
After renaming C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to ost-config.php and removing all after clicking "Disable Inheritance," 2)Click "Add" to add new permissions and click "Select a principal" 2) Type the user or group 3) Click "Check names" and 4) Then click "Ok". From there, you will click Apply and Ok where and see the change for the permissions.
</p>
<br />

![image](https://github.com/user-attachments/assets/b638c008-ebc7-4900-b8f1-dfc25bce6746)

<p>
In osTicket Installation Files folder, 1)Install HeidiSQL 2) After installation, right-click on "Unnamed" to create a new Database 3) After typing "osTicket" as the Database, it will show up here. After this process, it will show that the osTicket Installer was successfully installed.
</p>
<br />

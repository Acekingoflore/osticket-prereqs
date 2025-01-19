# osticket-prereqs
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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/G54blYV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First we create an Azure Virtual Machine Windows 10, 2 vCPUs (at least 2 vCPUs for better performance of the virtual machine) Then call the VM whatever name you like. I will be calling it osticket-vm, then create a username, then password. For me it will be labuser as the username and osTicketpassword1! As the password then
Log into the VM with Remote Desktop (Windows App).

Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop by right clicking and click extract all. The folder should be called “osTicket-Installation-Files” just make sure when you extract it that it's going to the osTicket-Installation-Files folder.
We will use the files in this folder to install osTicket and some of the dependencies to make sure the app is working as it should.


Install / Enable IIS in Windows WITH CGI
Go to control panel in the start menu and then you click on uninstall programs (Programs) 
Then on the left you should see turn windows feature on or off (click it)
Then within the small box that came up look for internet information Services then expand
Then look for World Wide Web Services then expand that as well
From there you should see Application Development Features expand it
Then you should see CGI, make sure to check the box, then hit ok.
Then the web server should be installing once finish close the box.




Now From the osTicket-Installation-Files folder, install PHP Manager for IIS double click 
(PHPManagerForIIS_V1.5.0.msi) a window will pop just hit next, hit agree, then then hit next again. Then say yes to everything, then let it install, now hit close.


From the osTicket-Installation-Files folder install the Rewrite Module (rewrite_amd64_en-US.msi) the same folder we downloaded the PHP Manager. Accept terms then hit install and say yes to everything. 


Now we are going to create the directory C:\PHP. click on the file explorer then go to windows (C:) Drive, it will be in This PC and just hit the drop down arrow on the left then make a folder within the drive and name it PHP. Then go back into the  osTicket-Installation-Files folder and then right click on PHP 7.3.8 file and extract all and when the window pops up. To make sure the contents of the file go to the right file hit browse on the window box that came up and go to the window (C:) drive and double click of the PHP file we created earlier and then select it and then hit extract.




From the osTicket-Installation-Files folder, install VC_redist.x86.exe. Then 
From the osTicket-Installation-Files folder again, double click MySQL 5.5.62 (mysql-5.5.62-win32.msi) Then accept terms and hit next. Choose Typical Setup then, hit install.
Launch Configuration Wizard (after install) -> hit next
Standard Configuration -> hit next 
We will make a simple and easy password and username just make it the username and password below. Feel free to make a note of the username and password
Username: root
Password: root
Then hit next and then execute

Then you should be at this image above so far.

</p>
<br />

<p>
<img src="https://i.imgur.com/G35mRip.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Software and Technologies Used</h2>

- Windows 10</b> (21H2)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

<h2>List of Prerequisites</h2>

- Create a Virtual Machine in Azure
- Install osTicket v1.15.8
- Install HeidiSQL
- Install MySQL
- Install PHP
- install Microsoft Visual C++ Redistributable

<h2>Installation Steps</h2>
<p>
  <img src="https://github.com/user-attachments/assets/ece03131-8dec-4fe7-a523-7f27a9a2bf15"/>
</p>
<p>
Let’s start by creating our Windows 10 Virtual Machine (VM). I like to use one that has at least 2CPUs.  Make a note of the username and password you choose. Lastly, be sure to let Azure create a new virtual network (Vnet)
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/894d1bd8-331c-4cf6-941f-c17f9646528b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open your Remote Desktop Connection app on your computer and connect to your Virtual Machine that was created in Azure.</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/feac83fe-b960-4d56-a75f-6689cb04c33d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Be sure to extract the folder so all the contents are on your desktop</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b5865fce-0849-4437-8114-c1afe6b04db8" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we need to install / Enable IIS in Windows. Go to your Search Bar > Type "Control Panel" > Click "Programs" > "Turn Windows features on or off" > Scroll down to "Internet Information Services (IIS).  Expand it and then expand the "World Wide Web" tab. Afterward, expand the application Developer tab. Finally check the "CGI" button & press Ok. You will need CGI to download the PHP Manager. The PHP manager is a back-end web programming language that allows osTicket to run off a web browser.
<br />

<p>
<img src="https://github.com/user-attachments/assets/5449f826-ed94-45ca-aef4-08f6c88abd6c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download the PHP manager file, and agree with all the terms and it should now be installed onto the virtual machine.
<br />

<p>
<img src="https://github.com/user-attachments/assets/19ff40c6-eefa-4da9-ba29-7cee5ad22bfc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download the Rewrite Module file, agree with all the terms and it should now be installed onto the virtual machine.
<br />

<p>
<img src="https://github.com/user-attachments/assets/cc68df1e-5381-4489-8c46-7aaf1a6eeac5" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Explorer, type, "C:\" in the search bar, and create a new folder called “PHP”. Download php-7.3.8-nts-Win32-VC15-x86.zip and unzip this folder’s contents into the PHP folder.
<br />

<p>
<img src="https://github.com/user-attachments/assets/1112263f-fa5d-4140-a4b8-11d8597f14cd" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agree to the terms and it will be installed.
<br />

<p>
<img src="https://github.com/user-attachments/assets/3032a422-eb7c-44d8-bbb6-7ef919399bbe" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install MySQL
<br />

<p>
<img src="https://github.com/user-attachments/assets/e48ff433-ca90-4c59-8a6a-4255e0e59c67" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
extract contents from osticket zipped folder. it will have two folders “scripts, & upload”
<br />

<p>
<img src="https://github.com/user-attachments/assets/3c8dd66d-b1dd-4b56-a30c-964afd7adaaf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Move the “upload” folder into “C:\inetpub\wwwroot” and rename it to “osTicket”
<br />

<p>
<img src="https://github.com/user-attachments/assets/1e439dd6-b8c5-4171-9121-1be66418618d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload ISS by stopping & starting the server
<br />

<p>
<img src="https://github.com/user-attachments/assets/69f87051-1d38-4838-97a1-5dd5254d9257" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the osTicket site by going to sites -> Default -> osTicket & then clicking on “Browse *:80(http)” on the right side of the screen.
<br />

<p>
<img src="https://github.com/user-attachments/assets/dad74857-3e2e-4cff-8e5c-7d8264abcead" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the osTicket site by going to sites -> Default -> osTicket & then clicking on “Browse *:80(http)” on the right side of the screen.
<br />









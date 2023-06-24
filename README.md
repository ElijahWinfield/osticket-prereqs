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

- PHP Manager for Internet Imformation Services (IIS) - (External Download) - https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link
- Rewrite Module - (External Download) - https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link
- VC_redist.x86.exe - (External Download) https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link
- PHP 7.3.8.ZIP - (External Download) https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link
- MySQL 5.5.62 - (External Download) https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link
- osTicket v1.15.8 - (External Download) https://drive.google.com/file/d/1VeVXKlzHDRjeaVUL99ptq7qYbrbXdFxJ/view?usp=drive_link
- HeidiSQL - (External Download) https://docs.google.com/document/d/1WovrX2DaS9xkfaSr4LXyB4YnnWpXIgPCMMbbfgHmGVw/edit


<h2>Login URL Links</h2>

- Help desk login page: http://localhost/osTicket/scp/login.php 

- End Users osTicket URL: http://localhost/osTicket/

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 1:
  *Install / Enable IIS in Windows WITH CGI and Common HTTP Features*
  1.  Click on the windows start menu logo
2.  Type Control Panel in the search bar located at the top of the window
3. Click on the control panel Icon or App
4. Click on Programs that is highlighted in green
5. Click on turn windows features on or off that is highlighted in blue next to a shield icon
6. Once that window pops up, Scroll or look until you see Internet Information Services
7. Check the Internet Information Services box (IIS) 
8. Click on the + Symbol next to where it says Internet Information Services
9. On that dropdown you want to look for where it says World Wide Web Services
10. Click the + Symbol next to World Wide Web Services
11. On that dropdown you want to look for where it says Application Developmet Features
12. Click the + Symbol next to Application Development Features
13. Check the CGI Box
14. Press the - Symbol next to Application Development Features
15. Click the + Symbol Next to Common HTTP Features
16. Check off all the boxes inside of it
17. Click ok and then close everything
18. Open up a web browser and type 127.0.0.1 and press enter to check

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 2:
  *Download and installing PHP Manager for IIS and Rewrite Module*
  1. Download Link (PHP Manager for IIS) : https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link
  2. Download Link (Rewrite Module): https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 3:
  *Create the directory C:\PHP and install content into it*
  1. Download and install VC_redist.x86.exe. - https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link
2. Click on the folder Icon on windows
3. Click on this PC
4. Click on Local (C:)
5. Right Click an empty space and create a new folder called ‘PHP’
6. Download PHP 7.3.8 and extract the content into that new folder called ‘PHP’ - https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link



<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 4:
  *Downloading and installing MySQl server and setting up a Username and password*
  1. Download and install MySQL 5.5.62
2. MySQL Server Instance Configuration: Click on Standard Configuration
3. Click Next
4. Set New Root Username and Password
5. Username: root (example)
6. Password: Password1 (example)
7. Press Execute and then press finished when it is done




<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 5:
*Open IIS as an Admin > Register PHP from within IIS*
1. Click on the windows icon and search IIS
2. Right Click on the icon and run as ‘Admin’
3. Double Click on the PHP Manager Icon
4. Click on Register New PHP Version
5. Click on the 3 Dots Next to it
6. Browse to the PHP folder and inside it click on the php-cgi.exe
7. Reload the IIS Server



<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 6:



<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 7:



<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 8:


  <p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 9:


  <p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 10:


  <p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 11:


  <p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  STEP 12:


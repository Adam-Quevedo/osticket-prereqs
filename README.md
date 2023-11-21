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

- Windows 10</b>

<h2>List of Prerequisites</h2>

- Windows PC
- Internet Connection
- Azure Subscription
- 2 Virtual Machinces
- Item 5

<h2>Installation Steps</h2>

<p>
</p>
<p>

First we need to Enable "CGI" and "Commonn Web Features to allow support for CGI executables and Web Server Content inside the Virtual Machine.
  
  Step 1: Open the Control Pannel and search for Windows Features

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/875444b1-2242-41bb-a438-90e5ed68b0e2)

Step 2: Inside the  Windows Features list open the Internet Information Services (IIS) Folder --> World Wide Web Services  --> Application Development Features then Enable CGI

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/6592c481-c998-47fc-9a4b-d936da143ee3)

Step 3: Enable the Common HTTP Features by going from World Wide Web Services --> Common HTTP Features

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/fc3c7c06-ab47-4f80-8fca-0c818d5a32b4)

Once that is done we need to Enable Internet Information Services(IIS) Managment Console

Step 4: While still inside Windows Features under the IIS Folder is IIS Management Console, Check that Box. 

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/519f2d05-6799-4d95-8cde-3ac2ee0c861b)


  
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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

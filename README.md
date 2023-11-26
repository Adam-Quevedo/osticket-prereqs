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

Now everything is turned on, we can download and Install the necessary PHP Manager and Rewrite Module.

Step 5: Download both files and install them on the computer.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/de30c91a-9d7f-415b-9742-3c8b3510cac6)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/9a8dbfbe-1377-4150-972c-6afa27279d9b)

Next we can create a directory in our system named "PHP"

Step 6: Navigate to the C: drive on the computers file explorer.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/2cda8151-d707-4834-86d1-684d8d4e0737)

Step 7: Create a new folder named "PHP".

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/f801bd0c-9beb-4d51-9d5f-e313fe14afdc)

Step 8: Download PHP 7.3.8 and Unzip the file into the newley made PHP file inside the C: drive.

Step 9: Download and install both VC_redist.x86.exe and MYSQL 5.5.62 .

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/dca8c9a5-0e9c-4ac9-bebd-9529c963f204)


After everthing is installed we can configure the programs

Step 10: Once MySWL is installed launch the program and continue with a standard configuration with a secure reset password.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/52b55e0c-1cd3-46a9-b1bd-c7d6a985a93b)

Step 11: Open the Internet Information Services Management console on the computer as an Admin

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/b65d5a62-8d28-43f1-a90f-81be20a335d0)

Step 12: Inside the IIS open the PHP Manager system

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/63efb7b9-b6e9-4c74-b533-2a27c03c3f5a)

Step 13: Register PHP Version using the application file found inside the PHP folder on the C: Drive

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/87f918df-67f6-485b-a5fd-58c44632b5eb)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/215be707-707f-45a9-b318-4ed381e4bff0)

Step 14: Back out to tha main page on IIS and restart the server

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/a14118c8-11e7-49d0-8335-99f5d000d345)








  
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

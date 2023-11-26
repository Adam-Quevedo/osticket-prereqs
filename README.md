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

<h2>Installation Steps</h2>

<p>
</p>
<p>

Before we do anything, we need to remote desktop into the virtual machine using the Ip address.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/c3b95c4e-f822-49ce-bdde-e8914d891ea8)


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

Step 11: Open the Internet Information Services Management console on the computer as an Admin.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/b65d5a62-8d28-43f1-a90f-81be20a335d0)

Step 12: Inside the IIS open the PHP Manager system.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/63efb7b9-b6e9-4c74-b533-2a27c03c3f5a)

Step 13: Register PHP Version using the application file found inside the PHP folder on the C: Drive.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/87f918df-67f6-485b-a5fd-58c44632b5eb)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/215be707-707f-45a9-b318-4ed381e4bff0)

Step 14: Back out to tha main page on IIS and restart the server.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/a14118c8-11e7-49d0-8335-99f5d000d345)

Install OSTicket on the computer.

Step 15: Inside the OSTicket donwload folder drag the Upload folder to the wwwroot folder inside the intetpub foledr on the C: drive.

Step 16: Rename Upload folder to "OSTicket".

Step 17: Inside IIS on the dropdown menu on the left open the Open the Sites Tab  --> Default Web Site --> OSTicket .

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/669c20af-08cf-4413-b5c8-d7c62284dea8)

Step 18: Click Browse *80 (http)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/bf2b33e3-48f4-4df7-8192-294239168e4a)

--Keep this on the side--

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/3b38fca0-d5ce-44f9-94be-81bef0181018)



We now need to turn on some extensions to help OSTicket.

Step 19: On IIS in the OSTicket page go to "PHP Manager" and then "enable or disable extenstions".

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/91a628f4-2382-418f-831a-87d197e6ce51)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/8015384d-5a83-4af2-a47a-28f3c9a223a1)

Step 20: Inside enable all of these extensions: --php_imap.dll --  php_intl.dll -- php_opcache.dll

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/304facc8-867f-4191-a8e1-6524b3a199c9)


Step 21: Inside the previous wwwroot folder in file explorer open the OSTicket folder --> include, rename the -- ost-sampleconfig.php -- to -- ost-config.php --

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/c06987ef-af7d-48dd-a95a-88f5432b0975)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/65772fea-35c1-488c-aa81-a988c959537b)

Step 22: Open the Properties on the renamed file go to security --> Adavnced and Disable Ingeritance. Remove all Permissions when the pop-up appears.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/b711d7c7-c654-40be-a511-5edb6ea0dab1)

Step 23: Once done, Click add permission --> select a principal --> Type everyone in the textbox and clich Check Names --> Ok. Then check off Full Control then Ok.

We can now go back to the Browser with OSTicket and click Continue.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/0bc953f1-52ad-401e-ab9a-218a430fbe7a)

Step 24: Fill out all the information needed in the System Settings and Admin User

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/1a048544-bce0-40ef-8444-0380d7f5fe25)

Step 25: On the side, Install HeidiSQL and open the Application.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/e8908349-7a0e-46e9-a3c7-43d02d554a4f)

Step 26: Inside HeidiSQL Start a new Session.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/fe975b30-049e-4d04-89d1-380c03ed84a6)

Step 27: Using the Login Info from MySQL type that in the respective boxes and Open.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/f576f710-cff6-405a-bdb4-f158237043cb)

Step 28: Right Click on Unamed and create a new Databade named OSTicket

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/3c31f9d8-d7a7-493e-90d5-0061556c7fb0)

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/f8fb87dd-ba97-498c-b818-955d1c1384a5)

Step 29: Back on the browser with OSTicket Type all the info needed in the Database Settings using the info we made in MySQL and HeidiSQL.

![image](https://github.com/Adam-Quevedo/osticket-prereqs/assets/151606017/11ffedf1-6297-4345-90c9-4c58583dd199)

Step 30: Click Install Now.

OSTicket is Fully Installed and we are ready to Clean up anything left over.

Clean Up: Go to the C: Drive --> inetpub --> wwwroots --> osTicket  --> setup and delete the folder

Clean Up: C: Drive --> inetpub --> wwwroots --> osTicket --> include --> ost.config.php Set the file to read only in the permissions

You can now go to http://localhost/osTicket/scp/login.php to login.



  
</p>
<br />


<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10, 4 vCPUs
- Install / Enable IIS in Windows WITH CGI and Common HTTP Features
- IIS Management Console
- Open IIS as an Admin
- Install osTicket v1.15.8

<h2>Installation Steps</h2>


![image](https://github.com/mkpene/osticket-prereqs/assets/142267681/b5cf0da2-a2af-4e53-9f31-7f1cf1dac131)

<p>
After setting up a Windows virtual machine, I opened the "Add or Remove Programs" settings and turn on the "Internet Information Services" feature. This would install IIS on the system. Once IIS is installed, I opened the IIS Manager. From there, I navigated to the server node and selected "ISAPI and CGI Restrictions." I'd add a new restriction and specify the path to the CGI executable. 
</p>
<br />


![image](https://github.com/mkpene/osticket-prereqs/assets/142267681/fe2d6f1f-b6ed-4d4d-8072-da4ca548b59a)

<p>
Once the installer was downloaded, I ran it and followed the installation wizard's steps. I opted for the complete installation since I wanted access to all the features. During the setup, I was prompted to set a root password, which I made sure was strong and memorable. Also went ahead and configured the settings to be amiable with OS Ticket.
</p>
<br />


![image](https://github.com/mkpene/osticket-prereqs/assets/142267681/6f0af408-ce3d-490e-94ac-32d09a427057)

<p>
By this point in the installation process I created a new virtual host configuration for osTicket. I made sure to set the document root to the location where I extracted the osTicket files. With the web server ready, I opened my browser and navigated to the URL of my virtual host. This triggered osTicket's installation script. I followed the prompts, setting the appropriate database information (database name, user, password) when prompted. The script automatically created the necessary tables in the database. Inside the admin panel, I navigated to the settings section. I configured the basic settings like the support email address, organization details, and default ticket setting for the project guidelines.
</p>
<br />

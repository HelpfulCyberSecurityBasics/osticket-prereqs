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

- Microsoft Azure account: Used to create and manage the virtual machine where osTicket will be installed.
- Virtual Machine (VM): A Windows 10 Pro VM with at least 2 vCPUs and 8 GB of RAM is required to host osTicket.
- Remote Desktop Connection: Essential for accessing and managing the virtual machine.
- osTicket Installation Files: These are provided as a downloadable ZIP file, containing all necessary components and dependencies for osTicket.
- Internet Access within VM: Needed to download the osTicket installation files and other necessary software.

<h2>Installation Steps</h2>

<p>
<img width="940" height="396" alt="Screenshot 2026-02-01 at 10 18 03 AM" src="https://github.com/user-attachments/assets/8b72b2a4-e413-4f74-823a-fa02638a7c11" />

</p>
<p>
1. Virtual Machine Setup:

- Create a virtual machine in Microsoft Azure.
- Configure the VM with Windows 10 Pro, 2 vCPUs, and 8 GB RAM.
- Set up username (NX user) and password (osTicket password one!) for the VM.

</p>
<br />

<p><img width="616" height="367" alt="Screenshot 2026-02-01 at 10 22 54 AM" src="https://github.com/user-attachments/assets/9520adb6-d672-4c5a-87ce-22a32a6758b1" />
<img width="774" height="419" alt="Screenshot 2026-02-01 at 10 25 22 AM" src="https://github.com/user-attachments/assets/480dea54-63b9-4557-b043-90718d8d25c7" />
<img width="756" height="417" alt="Screenshot 2026-02-01 at 10 27 01 AM" src="https://github.com/user-attachments/assets/dab8e55b-8c31-4871-b5af-9bbbd35e4052" />


</p>
<p>
2. OS Ticket Installation Files and IIS/PHP Setup:

- Connect to the VM using Remote Desktop Connection.
- Download osTicket installation files from the provided GitHub link.
- Extract the downloaded files to the desktop.
- Install and enable IIS (Internet Information Services) by turning on Windows features.
- Install PHP management and rewrite.
- Create a PHP folder in the C: drive and extract the PHP zip folder into it.
- Install VC Redist and MySQL.
- Configure MySQL instance and set root password.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. OS Ticket Configuration and Database Setup:

- Register the new PHP version in IIS manager.
- Stop and start the IIS server to restart it.
- Extract the osTicket zip folder into the wwwroot directory and rename it to "osTicket".
- Rename ost-sample-config.php to ost-config.php within the osTicket include folder.
- Set permissions for ost-config.php to "Full Control" for "Everyone".
- Continue with osTicket configuration in the browser, filling in help desk and admin user details.
- Install HeidiSQL.
- Create a new database named "osTicket" in HeidiSQL.
- Complete the installation by entering the database details (osTicket, root, root) and clicking "Install Now".
</p>
<br />

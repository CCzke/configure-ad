<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1> Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Active Directory Domain Services
- Remote Desktop
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create the Domain Controller VM
- Create Admin and Normal User account in AD
- Setup Remote Desktop 
- Create a lot of additional users 

<h2>Deployment and Configuration Steps</h2>

<p>
  
![IMG_1315](https://github.com/CCzke/configure-ad/assets/146891429/1989c9c3-9093-4c7e-b868-357a81856fe9)


</p>
<p>
The Domains Controller VM was created then the client VM made sure the client network was in the domain vnet and changed the NIC ip configuration to static, in this image i was in the domains desktop which only has the server manager.
</p>
<br />

<p>  
![IMG_1317](https://github.com/CCzke/configure-ad/assets/146891429/2fd06c56-a358-4014-a541-64a058ef5ba0)

</p>
<p>
With the AD running, I went to Active Directory users and computers to create some organizational units and then created a user for a specific unit and made it an Admin.
</p>
<br />

<p>
  
![IMG_1318](https://github.com/CCzke/configure-ad/assets/146891429/e40f07ef-f8a2-4492-a415-84cffc72ad3e)

![IMG_1322](https://github.com/CCzke/configure-ad/assets/146891429/7efaf338-1488-4a47-bbac-e52effe1a92a)


</p>
<p>
Lastly after setting up remote desktops to all domain users open Powershell create a new file, paste the contents of a script, and let it run so many accounts are created.
</p>
<br />

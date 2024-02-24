<p align="center">
<img src="https://imgur.com/dRUt1rz.png" height="40%" width="40% alt="Microsoft Azure Logo"/>
</p>

<h1>Creating Virtual Machines on Azure</h1>
This tutorial outlines the creation and use of Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- PowerShell

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Sign up for an Azure account - https://azure.microsoft.com/en-us/free/
- Create a Resource Group
- Search for Virtual Machines
- Configure and Create the VM in Azure
- Log on to the virtual machine

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/Ul8WLDn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<img src="https://i.imgur.com/OhIATkw.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/GE28xnW.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>

</p>
<p>
The first step is to create a Resourse Group. In Azure, a Resource Group serves as a place to keep all of your related resources together. Think of it as a folder. The virtual machine we will create will be placed inside of this resource group.
</p>
<br />

<p>
<img src="https://i.imgur.com/k41Jd8v.jpeg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<b />
<img src="https://i.imgur.com/nDZ2ASF.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create and name your resource group. In this example, the resource group was named "Azure_Virtual_Machine". Next, choose the region you want your resource group to be created in. Keep in mind, depending on the region you choose, Azure options may adjust or not be available. In this example (US) East US 2 will be chosen. Click "Review + Create" at the bottom of the page and create the resource group. 
</p>
<br />

<p>
<img src="https://i.imgur.com/hsWzYdD.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the Azure menu and select Virtual Machine. There are other ways to find virtual machines such as typing it into the search bar above. On the next page, click create and select Azure Virtual Machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/M4ILI10.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Configure your virtual machine by first selecting the resource group you created.
</p>
<br />

<p>
<img src="https://i.imgur.com/z1dkrau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<img src="https://i.imgur.com/fmcKE4Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Name your virtual machine, select the region, availablility options, Zones and image (Operationg System). The second image displays the most basic configuration for the virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/xtxlb9f.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select a size for the virtual machine. The sizes have different CPU sizes and memory and each cost a different amount.
</p>
<br />

<p>
<img src="https://i.imgur.com/CIUPT7i.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a username and password, click the check box to confirm licensing.
</p>
<br />

<p>
<img src="https://i.imgur.com/8qj6pBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p> 
<img src="https://i.imgur.com/KMxHufZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select the Network tab and confirm if a virtual network was assigned to your virtual machine. You could also create one if you choose to. Then select "Review + Create", if you have the desired settings then click "Create" located at the bottom of the page.

There will be a warning stating that the RDP port is open to the internet. Feel free to continue. RPD is needed to connect to your virtual machine.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/VN78QOG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Allow the virtual machine to develop COMPLETELY before using the booting the machine. After completed, click "Go to Resource" to be taken to your vitual machine page.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/cHI4ypE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
So now you created a virtual machine. Not it's time to use RDP to log into the virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/eoBHqkI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<img src="https://i.imgur.com/rk2pEpq.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
In order to use the virtual machine you would need to copy the virtual Public IP address as shown above. On the taskbar, search and select "Remote Desktop Connection". 
</p>
<br />

<p>
<img src="https://i.imgur.com/YgKSC4K.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enter the virtual machine's Public IP Address and connect.
</p>
<br />

<p>
<img src="https://i.imgur.com/z4uvNKU.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<img src="https://i.imgur.com/HVHQ3rQ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
 
</p>
<p>
On the Windows Security pop up screen, click "More choices", then select "Use a different account". Input the Username/password you created during the configuration of the virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/w2hyDF8.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lastly, a warning window may pop up explaining that there were errors validating the certificate of the virtual machine. That is from the type of security chosen during the configuring of the virtual machine. Proceed and click yes to start the virtual machine.

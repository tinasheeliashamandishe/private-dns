<h1>Azure Private DNS</h1>

<h2>Description</h2>
This lab will configure Azure Private DNS.<br /><br />

Azure Private DNS is a service that allows you to manage and resolve DNS names within a virtual network (VNet) in Azure. It enables you to create and manage private DNS zones that are only accessible within your Azure environment, making it ideal for internal applications and services.<br /><br />


Key Features of Azure Private DNS:<br />

<b>Private DNS Zones:</b> Create DNS zones that are not accessible from the public internet, allowing you to define and manage domain names used by your applications.
<br />
<b>Integration with Virtual Networks:</b> Automatically resolve DNS names for resources within the same virtual network or across peered VNets, facilitating seamless communication.
<br />
Custom DNS Records: Supports various DNS record types, including A, AAAA, CNAME, and TXT, allowing you to tailor the DNS configuration to your needs.
<br />
Private Link Integration: Works well with Azure Private Link, allowing you to connect services privately without exposing them to the public internet.
<br />
DNS Resolution: Provides efficient DNS resolution for resources within Azure, reducing latency and improving performance for internal applications.
<br />
Access Control: You can control access to DNS zones and records, ensuring that only authorized users and services can manage DNS configurations.
<br />
Hybrid Connectivity: Supports hybrid cloud scenarios, allowing integration with on-premises DNS solutions using VPNs or Azure ExpressRoute.


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Topology</h4>
Below, we have created a VM. This VM has no public IP address. Ware going to use Azure to log onto the VM<br/>
<img src="https://i.imgur.com/bhbcrm3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h4>Step 1</h4> 
Create a Bastion subnet.<br/>
<img src="https://i.imgur.com/M5MkGaP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h4>Step 3</h4> 

<h4>Step 2</h4> 
Configure Bastion.<br/>
<img src="https://i.imgur.com/YnUlt3I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h4>Step 3</h4>

<h4>Step 3</h4> 
Log into the VM.<br/>
<img src="https://i.imgur.com/tmw9F3Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Vtbz3yY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h1>Azure Private DNS</h1>

<h2>Description</h2>
This lab will configure Azure Private DNS.<br /><br />

Azure Private DNS is a service that allows you to manage and resolve DNS names within a virtual network (VNet) in Azure. It enables you to create and manage private DNS zones that are only accessible within your Azure environment, making it ideal for internal applications and services.<br /><br />


Key Features of Azure Private DNS:<br />

<b>Private DNS Zones:</b> Create DNS zones that are not accessible from the public internet, allowing you to define and manage domain names used by your applications.
<br />
<b>Integration with Virtual Networks:</b> Automatically resolve DNS names for resources within the same virtual network or across peered VNets, facilitating seamless communication.
<br />
<b>Custom DNS Records:</b> Supports various DNS record types, including A, AAAA, CNAME, and TXT, allowing you to tailor the DNS configuration to your needs.
<br />
<b>Private Link Integration:</b> Works well with Azure Private Link, allowing you to connect services privately without exposing them to the public internet.
<br />
<b>DNS Resolution:</b> Provides efficient DNS resolution for resources within Azure, reducing latency and improving performance for internal applications.
<br />
<b>Access Control:</b> You can control access to DNS zones and records, ensuring that only authorized users and services can manage DNS configurations.
<br />
<b>Hybrid Connectivity:</b> Supports hybrid cloud scenarios, allowing integration with on-premises DNS solutions using VPNs or Azure ExpressRoute.


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Topology</h4>
Below, we have created a VN. This VN has 2 subnets. <br/>
We will configure an azure private dns service, so that resources in the VN can communicate using FQDNs.<br/>
<img src="https://i.imgur.com/EJ6N21j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h4>Step 1</h4> 
Create a Private DNS Zone.<br/>
<img src="https://i.imgur.com/hlsO0PS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h4>Step 3</h4> 

<h4>Step 2</h4> 
In your private DNS Zone. Link it to your VN.<br/>
<img src="https://i.imgur.com/TtmcQnQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/q5ap1Dy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
Use auto registration to ensure that your VMs are automatically aded to the record sets.
<img src="https://i.imgur.com/2PEsAfV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<h4>Step 3</h4> 
After the setup is doen your VMs can communicate using FQDNs..<br/>
<img src="https://i.imgur.com/HkfDJ4W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


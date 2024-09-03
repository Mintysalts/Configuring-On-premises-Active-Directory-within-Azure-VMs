<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Setup Resources in Azure</h2>
1. Create the Domain Controller VM (Windows Server 2022) named “DC-1” (Take note of the Resource Group and Virtual Network (Vnet) that get created at this time)

2. Set Domain Controller’s NIC Private IP address to be static

3. Create the Client VM (Windows 10) named “Client-1”. Use the same Resource Group and Vnet that was created in Step 1.a

4. Ensure that both VMs are in the same Vnet (you can check the topology with Network Watcher


<h2>Ensure Connectivity between the client and Domain Controller</h2>
5. Login to Client-1 with Remote Desktop and ping DC-1’s private IP address with ping -t <ip address> (perpetual ping)

6. Login to the Domain Controller and enable ICMPv4 in on the local windows Firewall

7. Check back at Client-1 to see the ping succeed







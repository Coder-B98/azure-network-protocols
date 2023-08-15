<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a resource group with two virtual machines in Microsoft Azure one should have Windows 10 and the other should run Ububtu.
- Connect to the Windows virtual machine and use it to install wireshark
- Use wireshark to observe ICMP traffic.
- Use wireshark to observe SSH traffic.
- Use wireshark to observe DHCP traffic.
- Use wireshark to observe DNS traffic
- Use wireshark to observe RDP traffic.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/ck0r2pL.png"/>
</p>
<p>
Use Microsoft Azure to create two virtual machines. When creating the Ubuntu virtual machine set it to use a password as shown in the above screenshot.
</p>
<br />

<p>
<img src="https://i.imgur.com/VePiSNS.png"/>
</p>
There should be two virtual machines created as shown in the above screenshot. Conncect to the virtual machine running windows.
<p>
<br />
  
<p>
<img src="https://i.imgur.com/VePiSNS.png"/>
</p>
There should be two virtual machines created as shown in the above screenshot. Conncect to the virtual machine running windows.
<p>
<br />

<p>
<img src="https://i.imgur.com/poZlZkX.png"/>
</p>
<p>
Go to https://www.wireshark.org/download.html and install wireshark onto the windows virtual machine that was made in Azure.
</p>
<br />

<p>
<img src="https://i.imgur.com/AwMDD9g.png"/>
</p>
<p>
Once wireshark is installed click on ethernet to begin capturing the local traffic.
</p>
<br />

<p>
<img src="https://i.imgur.com/HwvIED8.png"/>
</p>
<p>
Type in icmp into the bar of wireshark to isolate traffic from the internet control message protocol (ICMP).
</p>
<br />

<p>
<img src="https://i.imgur.com/CMYlcUO.png"/>
</p>
<p>
Use the Azure portal to note the private IP of the Ubuntu virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/WVf7cK2.png"/>
</p>
<p>
Use command line to ping the Ubuntu virtual machine and note the traffic that appears in wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/aMwAFKd.png"/>
</p>
<p>
Type in Secure Shell (SSH) to isolate SSH traffic in wireshark.
</p>
<br />




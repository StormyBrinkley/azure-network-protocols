<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [Creating Two Virtual Machines in Azure: Windows and Linux](https://youtu.be/hWDgydFGzGc?si=nAzxxpBrWnA6eQKX)
In this comprehensive video tutorial (featuring instrumental music and no audio commentary), I will guide you through the entire process of creating two virtual machines in Microsoft Azure. We will set up one virtual machine with a Windows operating system and another with a Linux operating system. This tutorial will cover all the necessary steps and configurations to ensure both virtual machines are up and running smoothly.
<br/>
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

- Creating Virtual Machines
- Conducting Network Activities: Filtering Traffic with Various Protocols in Wireshark Using PowerShell

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/eeFtFsy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigating to through VM1's essentials to obtain the public IP Address to add to Microsoft Remote Desktop. 
</p>
<br />

<p>
<img src="https://i.imgur.com/pxHBwVx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Microsoft Remote Desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/NnNED4P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Adding VM1's public IP Address to Microsoft Remote Desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/Xz9lhwr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Logging into Microsoft Remote Desktop with the credentials add in Azure during VM setup.
</p>
<br />

<p>
<img src="https://i.imgur.com/iU6K7Ou.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/9pTt9Fm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Trying pinging VM2, since VM1 and VM2 have the same private IP address, some Linux commands didn't work properly. I did a workaround and used the public IP address to complete the lap.
</p>
<br />

<p>
<img src="https://i.imgur.com/0SvpyJt.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Creating a firewall rule that denys ICMP traffic.
</p>
<br />

<p>
<img src="https://i.imgur.com/9pTt9Fm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Filtering traffic by ICMP viewing results in Wireshark.
<br />

<p>
<img src="https://i.imgur.com/CWj1q6C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Filtering traffic by DNS viewing results in Wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/epWorgI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Filtering traffic by SSH viewing results in Wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/epWorgI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Connecting to VM2 from VM1 through secure shell (SSH).
</p>
<br />

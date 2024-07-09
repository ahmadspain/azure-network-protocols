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

- Windows 10 (22H2)
- Ubuntu Server 20.04

<h2>Actions and Observations</h2>


![image](https://github.com/ahmadspain/azure-network-protocols/assets/158358030/de253a20-6a25-4e62-85bd-5b9370aeb9c3)

<p>
Observing ICMP traffic on Wireshark.
</p>
<br />


![image](https://github.com/ahmadspain/azure-network-protocols/assets/158358030/60d04e12-397e-4350-968e-76bac54b7919)

<p>
In the photo above, we have "SSH'd into" our Unbuntu virtual machine as well as filterd for SSH traffic only. 
</p>
<br />

![image](https://github.com/ahmadspain/azure-network-protocols/assets/158358030/a880dc0e-191b-4e11-9e59-e29d548874fa)

<p>
Now we have attempted to issue our virtual machine a new IP address by using the "ipconfig /renew" command and are observing the DHCP traffic as a result.  
</p>
<br />

![image](https://github.com/ahmadspain/azure-network-protocols/assets/158358030/965253ea-0c6e-4875-a0e1-92231732fdbf)

<p>
Here we have filtered for DNS traffic. From within a command line, we used "nslookup" to see what google.com's IP address is.
</p>
<br />

![image](https://github.com/ahmadspain/azure-network-protocols/assets/158358030/1653c33d-f6d5-4be8-ae56-99e1887370c9)

<p>
Finally, we filtered for RDP traffic. Since the RDP (protocol) is constantly showing you a live stream from one computer to another, traffic is always being transmitted.

</p>
<br />

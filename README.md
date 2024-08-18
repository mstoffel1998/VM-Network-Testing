<p align="center">


![Azure virtual machine logo](https://github.com/user-attachments/assets/5e5cd689-5231-4fd2-8cf4-0d8531be3c9f)




<h1>Microsoft Azure Virtual Machine Network Testing and Utilization</h1>
This tutorial outlines the Ulilization and Network testing inside of the virtual machines..<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Powershell
- Wireshark

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Linux Ubuntu Server 24.04 LTS - x64 Gen2

<h2>List of Prerequisites</h2>

- Azure Resource Groups
- Virtual Machine I (Windows 10)
- Virtual Machine II (Linux Ubuntu Server 24.04 LTS - x64 Gen2)
- Wireshark Download

<h2>Utilization and Testing Steps</h2>

<p>


![Lab 2 Screenshot 3](https://github.com/user-attachments/assets/4f7e72ac-bceb-4fb0-a4ae-a48f5e6e8403)



</p>
<p>
Step 1: Connect to Virtual Machine One by using Remote Desktop Connection and Getting the IP address from our Azure Virtual Machine created in the prvious steps.
</p>
<br />

<p>
  
![Lab 2 Screenshot 5](https://github.com/user-attachments/assets/0f251327-672e-4b0a-95b9-ce0d683cc1db)


</p>
<p>
Step 2: Once in the virtual machine we will then go to a browzer and search and download Wireshark.
</p>
<br />


![Lab 2 Screenshot 6](https://github.com/user-attachments/assets/357e1685-fa23-4325-afdc-cc7e9195c681)


</p>
<p>
Step 3: We are going to go into wire shark and the first item of business is to check for ICMP Traffic on the channel. This will at first show no traffic, but one we ping for virtual machine Two by using its' IP address in Powershell, we should start getting traffic on Wirshark.
</p>
<br />

<p>
  
![Lab 2 Screenshot 9](https://github.com/user-attachments/assets/593e0bc5-50a9-47a4-9176-4bf7346f37e8)




</p>
<p>
Step 4: We will now check for RDP Traffic on wireshark by using Powershell and Searching for tcp port==3389 and hitting enter to see all of the RDP traffic due to the fact that we are using remote desktop to connect to Virtual Machine One.

</p>
<p>
Step 5: Be sure to clear out both Virtual Machines and the Resource groups to complete the project completely.

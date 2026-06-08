# azure-network-protocols<p align="center">
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

- Windows 11 (25H2)
- Ubuntu Server 24.04

<h2>High-Level Steps</h2>

- Deploy Cloud Infrastructure
- Capture and Analyze Network Traffic
- Configure and Test Network Security Controls
- Validate Connectivity and Protocol Behavior

<h2>Actions and Observations</h2>

<p>
<img <img width="1885" height="978" alt="Screenshot 2026-06-07 215004" src="https://github.com/user-attachments/assets/e551590e-5979-469e-9cf4-2b3e19ef7300" />

</p>
<p>
This screenshot shows the cloud infrastructure created within Microsoft Azure, including a Windows 10 virtual machine and an Ubuntu Linux virtual machine deployed within the same virtual network and subnet. This configuration enabled private network communication between the systems and provided a controlled environment for analyzing network traffic, connectivity, and security configurations.
</p>
<br />

<p>
<img <img width="1906" height="972" alt="Screenshot 2026-06-08 095916" src="https://github.com/user-attachments/assets/d0e857d7-2f49-4209-92fe-4388a7bc8e47" />

</p>
<p>
This screenshot shows Internet Control Message Protocol (ICMP) traffic captured within Wireshark during communication between the Windows 10 and Ubuntu virtual machines. ICMP echo requests and echo replies were generated using the ping command and analyzed to verify network connectivity between systems. This exercise demonstrated packet capture techniques, network troubleshooting, and protocol-level traffic analysis.
</p>
<br />

<p>
<img <img width="1884" height="975" alt="Screenshot 2026-06-08 101336" src="https://github.com/user-attachments/assets/e0802beb-ed06-43d9-ab50-90dc75cb6644" />

</p>
<p>
This screenshot demonstrates the impact of Azure Network Security Group (NSG) firewall rules on network communication. Inbound ICMP traffic was blocked on the Ubuntu virtual machine, causing ping requests from the Windows virtual machine to fail. After re-enabling the rule, connectivity was restored. This exercise demonstrated firewall administration, traffic filtering, access control, and the effect of security policies on network communications.
</p>
<br />

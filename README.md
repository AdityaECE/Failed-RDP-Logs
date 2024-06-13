# Failed-RDP-Logs
This project displays on how to work with Microsoft Azure Sentinel a SIEM tool to extract data and represent it on a map, indicating the number of failed login attempts on a virtual machine

# Description
The PowerShell script in this repository was responsible for parsing Windows Event Log information for failed RDP attacks and using a third-party API to collect geographic information about the attackers' locations.
I set up Azure Sentinel (SIEM) and connected it to a live virtual machine acting as a honeypot. We observed live RDP brute force attacks from around the world. Using a custom PowerShell script, I looked up the attackers' geolocation information and plotted it on an Azure Sentinel map.

# Azure Virtual Machine and Logs Analytics Workbook
Vitual Machine

<img width="949" alt="virtual machine" src="https://github.com/AdityaECE/Failed-RDP-Logs/assets/89286686/0b522380-3e3c-455f-ae6a-2e4ddfe46a0d">



Log Analytics Workbook

<img width="944" alt="log analytics workbook" src="https://github.com/AdityaECE/Failed-RDP-Logs/assets/89286686/25621514-cd56-4ee5-9fce-b669ec6aa763">

# Language Used
Powershell: To extract failed rdp logs from windows event viewer from VM

# Other Websites used
ipgeolocation.io : To get the Latitude and Longitude Information of attacker

# Virtual Machine Powershell 
<img width="683" alt="virtual machine powershell script and host logins pic" src="https://github.com/AdityaECE/Failed-RDP-Logs/assets/89286686/0923dcff-5b91-4b5a-8e43-01b26531c019">


This Powershell code is in the repository with the name of "Custom log exporter"


# Visual Representation of attacker's geolocation on Map
<img width="631" alt="failed rdp worldmap" src="https://github.com/AdityaECE/Failed-RDP-Logs/assets/89286686/b4ae2ab4-591b-4f54-a971-78e50a833ed6">

This data was collected within 1 hour

# Playbook to Add Malicious IP Addresses from Incident Entities to FortGate Firewall.
This readme document provides step-by-step instructions on how to add malicious IP addresses to FortiGate firewall, then put those IP addresses into an Address Group for FortiGate to apply policies to.

## Developed by 
* Naveen Kishore
* Sydney John Dsouza
* Vestal Michael
* Dinesh Kumar

## Prerequisites
1. Fortigate firewall is already configured with publically routable and SSL enabled URL.This URL will be used to send HTTP requests from Azure Logic app.
2. Make sure you a bearer token from an Administrator account created with right permissions assigned to it on Fortigate firewall.
3. Create a group / folder on FortiGate firewall under Policy & Objects --> Addresses.

## Deploy Azure Logic App

If you want to deploy this app to your Azure tenant, just click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FNaveen-SWO%2FAddIPtoFortiGate%2Frefs%2Fheads%2Fmain%2Ftemplate.json)

## Description of Actions Used in this Logic App
- **Microsoft Sentinel Incident** action uses an API connection to connect to your Sentinel Log Analytics Workspace when you manually trigger this playbook for an incident.  
  ![1. Microsoft Sentinel Incident Action](/Screenshots/1.Microsoft_Sentinel_Incident.jpg)

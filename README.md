# Playbook to Add Malicious IP Addresses from Incident Entities to FortGate Firewall.
This readme document provides step-by-step instructions on how to add malicious IP addresses to FortiGate firewall then put those IP addresses into an Address Group for FortiGate to apply policies to.

## Prerequisites
1. Fortigate firewall is already configured with publically routable SSL enabled URL.
2. Make sure you a bearer token from an Administrator account created with right permissions assigned to it on Fortigate firewall.
3. Create a group / folder on FortiGate firewall under Policy & Objects --> Addresses.

Task 11: Setting Up and Interacting with a Free Cloud VM
Overview
This repository contains the steps and screenshots of creating a free VM in the cloud, connecting to it from Kali Linux, and performing basic network interactions.

Steps to Create and Interact with the VM
1. Create a Free Cloud Account
Signed up for a free account on Azure (or GCP/AWS).
Verified account and completed the setup process.
2. Create a Virtual Machine
Selected a free-tier VM configuration with the following:
OS: Linux (Ubuntu preferred)
Instance size: B1s (1 vCPU, 1 GiB memory) or equivalent
Region: Closest available region
Noted down the public IP address of the VM once it was up and running.
3. Allow Network Access
Configured firewall settings to allow inbound SSH (port 22) and ICMP (ping) traffic.
4. Ping the VM from Kali Linux
Opened terminal on Kali Linux and pinged the VM's public IP:
ping <VM Public IP>
5. SSH into the VM
Logged into the VM using SSH from Kali Linux ssh -i <path to the private key file> <username>@<VM Public IP>
Once logged in, ran the following command to display the network interfaces ip a
Captured the screenshot of the result.
6. Ping Public IP from the VM
Found the public IP of the Kali Linux machine.
From the VM, pinged the public IP ping <Your Public IP>
Captured the screenshot of the result.
7. Deleting the VM
Go to the "overview" section in Azure.
Then click on "Delete".

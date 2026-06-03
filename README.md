 # 📘 Networking Basics Lab
# 📌 Overview

This repository documents my learning and hands-on practice with fundamental networking concepts as part of my journey toward becoming an IT Support Technician and Cloud Engineer.

The project focuses on understanding how devices communicate over a network and how to troubleshoot common connectivity issues using Windows tools.

# 🎯 Objectives
*Understand core networking concepts (IP, DNS, DHCP)

*Learn how devices connect and communicate on a network

*Use Windows command-line tools for troubleshooting

*Build practical IT support skills

# 🌐 Key Networking Concepts

📍 IP Addressing

What an IP address is: An IP address (Internet Protocol address) is a unique number assigned to every device on a network.

Why devices need IP addresses: Without an IP address, devices wouldn't know where to send data. When you load a website, your device sends a request to the server's IP address, and the server sends the website back to your IP address.

Difference between public and private IPs: Your public IP is like your building's street address. Your private IP is like your flat number inside that building. The outside world only sees the street address — your router figures out which device (flat) the data should go to.

📸 Screenshot: My IP configuration

<img width="713" height="1089" alt="Screenshot 2026-06-03 165311" src="https://github.com/user-attachments/assets/7fa68e78-1908-42d0-8e49-7fda951aef94" />


🌍 DNS (Domain Name System)

How domain names are translated into IP addresses:

You type google.com in your browser

   Your device checks its local cache — to see if the site as been visited before If yes, it already knows the IP and skips ahead
   
  - If not, it asks your router's DNS resolver 
   
  - The resolver checks its own cache. If it doesn't know either, it starts asking around:
   
   - First it asks a Root DNS Server — "Who handles .com domains?"
     
   - The root server says "Go ask the .com TLD (Top-Level Domain) server"
     
   - The TLD server says "The authoritative server for google.com is at this address"
     
   - The resolver asks Google's authoritative DNS server — "What's the IP for google.com?"
     
   - Google's server replies: "It's 142.250.187.46"
     
 The resolver sends that IP back to your device
    
 Your browser connects to 142.250.187.46 and loads Google

Why DNS is important for browsing the internet: It makes the internet more easier to use

📸 Screenshot: DNS lookup test

<img width="389" height="483" alt="Screenshot 2026-06-03 173525" src="https://github.com/user-attachments/assets/7da4fadf-6c17-43e4-85a1-c064ea0f8a4a" />


📡 DHCP (Dynamic Host Configuration Protocol)

How devices automatically receive IP addresses:

DISCOVER — Your device connects to the network and broadcasts  to the whole network 

OFFER — The DHCP server hears this and responds offers an available IP from its pool

REQUEST — Your device formally requests that specific IP address 192.168.1.15.

ACKNOWLEDGE — The DHCP server confirms and give it other stuff like subnet mask

Role of DHCP server in a network:

-Assigning IP addresses automatically so no one has to configure them manually

- Preventing IP conflicts — it tracks which addresses are already in use so two devices never get the same IP

📸 Screenshot: DHCP details

<img width="789" height="1084" alt="Screenshot 2026-06-03 173614" src="https://github.com/user-attachments/assets/fbbafd6a-87ee-4b4d-a198-72067446873f" />


🚪 Default Gateway

What a gateway is: A gateway is the device that acts as the "exit door" for your local network. It's the point where traffic leaves your network and goes out to the internet (or another network). In most cases, your router is your gateway.

How it connects local networks to the internet: Your local network uses private IP addresses (like 192.168.1.x) which don't work on the public internet. The gateway/router bridges that gap by NAT (Network Address Translation) — it swaps your private IP for the router's public IP, when receiving it translates back to Private.

📸 Screenshot: Default gateway information

<img width="713" height="1089" alt="Screenshot 2026-06-03 165311" src="https://github.com/user-attachments/assets/5498af55-43ca-42aa-ac1e-6050a7470957" />



# 💻 Practical Command-Line Work

Commands used:

ipconfig

ipconfig /all

ping google.com

nslookup google.com

tracert google.com

🔧 What each command does:

ipconfig → Shows IP configuration

ping → Tests connectivity to a device or website

nslookup → Checks DNS resolution

tracert → Shows the path data takes to a destination


📸 Screenshot: Command practice results

(Insert screenshots of each command output here)



🚀 Next Steps

Build Active Directory Home Lab
Learn Windows Server basics
Practice user account management
Expand troubleshooting skills

📁 Author

Aspiring IT Support Technician & Cloud Engineer
Focus: Networking, Microsoft Azure, and IT Infrastructure

⚡ Pro tip (important)

When you upload screenshots:

Put them in a folder called screenshots/
Name them clearly:
ipconfig.png
dns-lookup.png
troubleshooting.png
[![](https://komarev.com/ghpvc/?username=Isaiah1&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->

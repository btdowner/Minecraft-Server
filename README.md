# Minecraft Server: Bedrock Edition Project

**Project Overview:**
---------------------
In this project, I decided to create and configure a Minecraft Server: Bedrock Edition. This project showcases my ability to set up a server, manage configurations, and troubleshoot issues to provide a stable, fun environment for my kids, friends, and family to play the game. While Minecraft Bedrock offers Realms to host your own Minecraft world for Multiplayer, it does have its drawbacks. It has a maximum of 11 players that can play at once, less control over player control, and a $7.99 monthly fee.  

**Prerequisites:**
-----------------
- A mini PC with a Quad-core processor, 4GB of RAM, a 10 GB SSD, and a NIC capable of at least 5 
Mbps.
- A Server Operating System.
- A Hypervisor.
- Minecraft Server files.
- A USB drive.
- A Mojang account and license to play Minecraft: Bedrock Edition.

**Objectives:** 
---------------
- Set up a Minecraft server on a local machine. 
- Configure internal port forwarding for multiplayer access. 
- Manage server resources and monitor performance. 
- Customize server settings for a unique gameplay experience. 
- Ensure server security and stability.

**Technologies Used:** 
----------------------
- Minecraft Server Software: Minecraft Bedrock Edition Server 
- Operating System: Linux Ubuntu Server
- Hypervisor: Proxmox
- Network Configuration: Internal port forwarding (port 19132) 
- Tools: Command line interface (CLI) for Ubuntu Server and Proxmox, SSH

**Project Steps:** 
------------------
1. Installing Linux Ubuntu Server.
   - Downloaded the latest version of Linux Ubuntu Server.
   - Installed and setup Linux Ubuntu Server on my local machine.
2. Installing Proxmox Hypervisor.
   - Downloaded the latest version of Proxmox.
   - Installed and setup Proxmox on Linux Ubuntu Server
   - Configured Proxmox resources for the Minecraft Server, including allocating needed Cores, RAM, and SSD space.
3. Installing Minecraft Server Software: 

o Downloaded the latest version of Minecraft server software (Bedrock/Java). 

o Installed and set up the server on my local machine. 

o Configured the server properties (e.g., max players, game mode, difficulty 

level). 



- open firewall on proxmox
- no ip in source ip
- router changes Ip address used ddns
- play while away from home

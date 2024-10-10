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
1. Installed Linux Ubuntu Server:
   - Downloaded the latest version of Linux Ubuntu Server.
   - Installed and setup Linux Ubuntu Server on my local machine.
2. Installed Proxmox Hypervisor:
   - Downloaded the latest version of Proxmox.
   - Installed and setup Proxmox on Linux Ubuntu Server
   - Created Proxmox container VM and configured resources for the Minecraft Server. This included allocating needed Cores, RAM, and SSD space.
3. Installed Minecraft Server Software: 
   - Downloaded the latest version of Minecraft server software (Bedrock/Java). 
   - Installed and set up the server in the Proxmox container. 
   - I started the server VM and launched the terminal to configure the server properties (e.g., max players, game mode, difficulty level). 
4. Configured home router for port forwarding, a DHCP reservation, and DDNS for internal and external gameplay: 
   - Created a DHCP reservation for the Minecraft server IP address so it can be accessed from multiple devices.
   - Set up port forwarding for internal port 19132 to allow multiplayer access.
   - Created a DDNS rule that allows external devices to access the server.
   - Created 2 versions of server access on each device for internal and external gameplay.
      - Internal: Configured device server settings with server IP address and port.
      - External: Configured device server settings with DDNS name and port.
   - Tested the connection with multiple devices while both on and off the local network to ensure smooth gameplay. 
5. Managing Server Performance: 
   - Monitored server performance to ensure smooth gameplay. 
   - Reallocated sufficient RAM and CPU for optimal server performance, considering the number of players that joined the server.
6. Ensuring Security and Stability: 
   - Implemented server rules and permissions to manage players during gameplay. 
   - Regularly backed up the server to prevent data loss.
   - Applied updates and patches to keep the server secure.  
7. Tested overall gameplay with multiple players. 
   - I joined multiple devices to the server at once, both internally and externally.
   - Re-tested VM for adequate processor, memory, and storage resources.

**Challenges Faced:**
---------------------
- Network Configuration Issues: Initially, there were difficulties in setting up port forwarding correctly, but through troubleshooting and research, I could resolve the issue. 
   - Issue 1: Port forwarding was not working for external gameplay. I discovered that when creating the port forwarding rule, you must leave the external (router) IP address blank. When a device is configured 
              with the router's IP address and port, it connects to the server automatically. Having the IP assigned in the rule was causing conflict.
   - Issue 2: Each time I changed the port forwarding rule to resolve the above issue, I would then power cycle the router to apply the changes. Ironically, the IP address assigned to the router by my ISP is 
              dynamic and changes each time the router is power cycled. After some research, I learned about DDNS and created a DDNS record for the server. This resolved the issue of changing the external IP 
              address.
   - Issue 3: Server Performance took some adjusting to manage for multiple players. It took re-balancing resources effectively, especially during peak hours.
 
**Project Outcome:**
--------------------
- The Minecraft server was successfully deployed with stable performance and a fun, engaging environment for my family and friends. The project helped me improve my skills in server configuration, router configuration, network management, and problem-solving. 

**Conclusion:** 
---------------
This project demonstrated my ability to set up and manage a multiplayer Minecraft server, showcasing skills that are applicable in IT, network management, and server Administration. 


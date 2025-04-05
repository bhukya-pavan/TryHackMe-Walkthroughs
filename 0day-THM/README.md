# Introduction

0day is a medium box on the TryHackMe platform. The box involves exploiting a website with shellshock and exploiting an outdated linux kernel

Scanning

To start our enumeration of the box we do an initial nmap scan. Using -sC for default scripts, -sV for version enumeration and -oA to output the results 

![2025-04-03_04-09](https://github.com/user-attachments/assets/3d03499b-4e54-43b1-8128-23829df30532)

The results of this nmap show 2 ports open:

port 80 which is a HTTP server.
Port 22 which is a SSH service

Our next step is to look into the HTTP server. Navigating there in the browser shows a site which looks like Ryan's portfolio page.
![image](https://github.com/user-attachments/assets/f2521554-1f6d-47f6-9d1a-d328cb8e40c7)

let’s enumerate this website and see what we can find

![image](https://github.com/user-attachments/assets/6225c5e3-abdf-4513-9802-4d4cd97afde6)

![image](https://github.com/user-attachments/assets/2fa14f5f-779b-4bb8-ab73-516e74ce3e87)

sudo nikto -h {target_ip}

![image](https://github.com/user-attachments/assets/0506f4cf-4705-4f83-827a-216d20bd8892)



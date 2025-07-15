This is a full walkthrough on how to beat the Pickle Rick CTF at TryHackMe. The objective of this writeup is to explain to the future me and to anyone else how I was able to solve this CTF and what tools I used

ENUMERATIONS WITH NAMP;

<img width="1129" height="778" alt="image" src="https://github.com/user-attachments/assets/07d4a8d3-96a3-4214-84ce-693e1af4f3e3" />
After Enumeration Nmap Scan Bring This Information 

1) port 22 is open and SSH service with OpenSSH 7.2p2,
2) Port 80 is running a HTTP service with Apache 2.4.18

Exploring the website;

<img width="1351" height="694" alt="image" src="https://github.com/user-attachments/assets/a76d1fc2-ed4e-47e8-83b1-c92299854403" />
In This Page Nothing Intrested TO GO Forward 
Lets explore in pagesources 
<img width="1117" height="696" alt="image" src="https://github.com/user-attachments/assets/81ec8c7c-1a77-4a1d-a758-6c97d4f0ae05" />

Found :
    Username: R1ckRul3s
Using Gobuster search hiden directories;

<img width="1540" height="776" alt="image" src="https://github.com/user-attachments/assets/27a97cab-29df-463c-8259-98978348ab87" />

<img width="1660" height="694" alt="image" src="https://github.com/user-attachments/assets/dc602bdd-ed7c-47f6-9fd0-5263a2e79f33" />

successful logging 

<img width="1543" height="722" alt="image" src="https://github.com/user-attachments/assets/1a2c3fd1-16dd-477b-a8a8-7f4387175d8d" />

<img width="1222" height="687" alt="image" src="https://github.com/user-attachments/assets/e888c620-614e-4f67-a21f-153eca3dba47" />








   







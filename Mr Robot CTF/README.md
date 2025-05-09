🔍ENUMERATION

➡️Nmap Scan
Start with a basic scan
![image](https://github.com/user-attachments/assets/f3d3af79-a850-46d8-bcb0-07d31ec4afc1)

📄 Scan Outpu
Port 22 — SSH is closed
Port 80, 443 — A web page running a search website

🌐 Web Enumeration

After identifying that port 80 is open, I pasted the target IP in the browser:

![image](https://github.com/user-attachments/assets/619de8d0-ed3a-491d-9b5a-cc584dadbaf9)

 Run a directory brute-force scan using tools like `gobuster or ffuf:

 ![image](https://github.com/user-attachments/assets/88d82d36-75f6-4526-a7a8-4a1d1ddd40fe)

 I found first key 
 
 ![image](https://github.com/user-attachments/assets/9fb6b5d8-7598-4ab8-97f8-1a78de772fd2)

 
 ![image](https://github.com/user-attachments/assets/f0915338-0451-4a8b-a6b6-b46cf68325bb)

 Continuing our search for the directories we found some base64 string in the license directory

 ![image](https://github.com/user-attachments/assets/65608cac-f767-48b1-8814-30c1d3a8127c)

Lets use Cyber chef to decode the string 
 ![image](https://github.com/user-attachments/assets/73d2c715-e09e-4efa-92e8-5e69485898cd)


 



 


 







am starting with nmap scan 

![image](https://github.com/user-attachments/assets/226f8945-03fb-422d-8d8b-fd33fda48780)

i found two open ports 

port 22 
port 80

In the address bar, type  the IP address

![image](https://github.com/user-attachments/assets/654aadcc-231c-48d7-98be-c470dbdfdef5)

 Directory Bruteforcing

 ffuf -u http://10.10.104.4/FUZZ -w /usr/share/wordlists/dirb/common.txt -e .php,.html,.txt


 ![image](https://github.com/user-attachments/assets/fe72e367-6c25-4ce5-9163-3a3dad5eefde)

 ![image](https://github.com/user-attachments/assets/0a27be03-8780-442c-a96a-ac95d495c5b5)

 

 



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

 dirsearch  -u http://10.10.104.4/assets/index.php 

 ![image](https://github.com/user-attachments/assets/1c73a05e-5cc8-407a-a195-abd905f6fed2)

 ![image](https://github.com/user-attachments/assets/001c7bbe-3d96-49cf-be84-f044a874572e)

 After discovering a command injection vulnerability, our next goal is to gain reverse shell access to the target machine

 

 Generating the Reverse Shell Payload:

 ![image](https://github.com/user-attachments/assets/96b70750-144a-4fa0-930c-aed9e4acae6d)

 ![image](https://github.com/user-attachments/assets/847a9a46-db5a-406e-947c-93979b00fbe6)

 ![image](https://github.com/user-attachments/assets/86fc5eba-5951-4fcb-8353-5fa49d24e231)

 ![image](https://github.com/user-attachments/assets/9c51bdfe-f615-443e-8c1d-a9ef23757982)
 







 

 



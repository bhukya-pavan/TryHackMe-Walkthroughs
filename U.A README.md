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

 

 ![image](https://github.com/user-attachments/assets/d2057cdf-12cf-4efa-aa27-bd0432ec6c16)

 ![image](https://github.com/user-attachments/assets/6fb533b7-ae7b-4bb9-b6cc-f2cce26e8c5d)

 ![image](https://github.com/user-attachments/assets/2930e18d-5622-4327-a4bb-971b31e3fe81)
 
 password : One?For?All_!!one1/A

 ![image](https://github.com/user-attachments/assets/62452b96-d4ce-4b28-9fb8-c6cf4ccd8159)

 THM{W3lC0m3_D3kU_1A_0n3f0rAll??}

 ![image](https://github.com/user-attachments/assets/a573839c-2762-415d-8229-99687f680644)

 ![image](https://github.com/user-attachments/assets/f288db10-fb37-4533-80e1-7616d55b3437)

 
![image](https://github.com/user-attachments/assets/9ba4563d-79bb-475b-9f3c-0ac51d4d78fd)

here i creat test.txt file [tmp > /tmp/test.txt]



![image](https://github.com/user-attachments/assets/8f5aff68-4d41-4543-9de8-69013048c39f)

is used to generate a new SSH key pair using the RSA algorithm.

![image](https://github.com/user-attachments/assets/a91d7433-8e3b-4efa-8f80-5e13dab2e301)

copy this file into deku@myheroacademia:/tmp$ sudo /opt/NewComponent/feedback.sh

![image](https://github.com/user-attachments/assets/2a8fe781-4f3a-457e-bfe8-ed59aace9b4b)









 



 


 

 



 







 

 



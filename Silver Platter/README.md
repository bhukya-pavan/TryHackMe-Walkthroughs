Silver Platter:

Enumertaion 

Nmap Scan


![image](https://github.com/user-attachments/assets/50efb0ad-795a-4105-b2bb-9aa7b19eb575)

SSH (22)
.Password auth is enabled

![image](https://github.com/user-attachments/assets/98577ffa-f36f-46f0-9ec6-5080a61dc45e)

Enumeration on Port HTTP(80)

![image](https://github.com/user-attachments/assets/11400e06-cebc-4e76-98cd-0941fabb8b82)

Dirsearch -u http://10.10.23.64

![image](https://github.com/user-attachments/assets/5f7413b3-89ac-46c3-a3bd-2ecebd5aa079)

nothing interesting 

![image](https://github.com/user-attachments/assets/4bf09fd2-28b6-4ef1-b26f-14014dd85de3)

![image](https://github.com/user-attachments/assets/ad6e4cc5-6c22-4730-8a24-e04f45264352)


→ Navigating to “http://IP_Machine:8080/silverpeas/” displayed the following login panel 

found loginpage 

![image](https://github.com/user-attachments/assets/2d8d77e3-4fcc-4a8a-80e8-1d8ce81f2e2c)

Gnerate passwordlist:  cewl http://10.10.162.195 > password.txt


![image](https://github.com/user-attachments/assets/cf68dd44-91f6-426b-9c91-432fb55e9cdb)


![image](https://github.com/user-attachments/assets/d7ea0113-f5c1-4cff-9b39-f45eb08ff8b2)

![image](https://github.com/user-attachments/assets/d1fdc570-ab39-4c10-adfe-cde907a92ca4)

(adipiscing)  password: Login successfully 

![image](https://github.com/user-attachments/assets/1c7bf272-9882-4024-a40e-d97471b60bbc)


so changed the ID parameter and got SSH credentials

![image](https://github.com/user-attachments/assets/46f9b354-623b-468c-a349-918ce8ac5879)

Username: tim

Password: cm0nt!md0ntf0rg3tth!spa$$w0rdagainlol

![image](https://github.com/user-attachments/assets/c8b1dc61-43fc-4b8e-ac10-5daaf8ca5cf7)

![image](https://github.com/user-attachments/assets/4e17acfa-f0e3-40e1-9e19-eb27b8460368)

THM{c4ca4238a0b923820dcc509a6f75849b}

Privilege Escalation

grep -Ri "password" /var/log/

![image](https://github.com/user-attachments/assets/d07374f8-f4cf-4074-86b0-66be977415b5)

passwords: _Zd_zx7N823/

![image](https://github.com/user-attachments/assets/24fb8034-cabd-41c0-a722-e48e08c88964)

![image](https://github.com/user-attachments/assets/7255eee2-51e7-4f34-8455-7ba6b99d6ed2)

THM{098f6bcd4621d373cade4e832627b4f6}





































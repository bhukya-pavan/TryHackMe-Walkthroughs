
I start with a Nmap scan:

![image](https://github.com/user-attachments/assets/c2553df2-62cb-43cb-aa70-176bc74ddd05)

Nmap discovered 2 open ports: port 22 (SSH) and port 80 (HTTP)

![image](https://github.com/user-attachments/assets/01f1a259-73ff-4381-9b94-7e20fc93e4aa)


directory brute forcing using ffuf we get a directory

ffuf -u http://10.10.3.146/FUZZ -e .php,.txt -w  /usr/share/wordlists/seclists/Discovery/Web-Content/raft-small-words.txt

![image](https://github.com/user-attachments/assets/d7ba86bd-e404-499d-9c36-7d88532dfd71)

Navigating to /spip/ directory we get another article called publisher

![image](https://github.com/user-attachments/assets/b57861fb-be37-4405-a280-58808cba5a2a)

![image](https://github.com/user-attachments/assets/ae740fd2-8458-4d42-89f8-61ac3bfb05ba)

![image](https://github.com/user-attachments/assets/2dde3ff6-3a4d-431b-a832-adb81ece93dc)


![image](https://github.com/user-attachments/assets/7aa61437-cb92-4d46-8c4c-25fe59aea9d9)


![image](https://github.com/user-attachments/assets/0837530f-6168-402f-bac3-8d9d56020bf9)

fa229046d44eda6a3598c73ad96f4ca5 



![image](https://github.com/user-attachments/assets/7d83395e-acdd-43f9-9bec-da0ccc45f1c7)

Copy the entire content of the id_rsa file, including the -----BEGIN RSA PRIVATE KEY----- and -----END RSA PRIVATE KEY----- lines.


On our local machine, create a new file and paste the copied RSA key into it


nano think_rsa

![image](https://github.com/user-attachments/assets/46bce293-9c5d-4335-a25d-2348cab1f534)

![image](https://github.com/user-attachments/assets/4fe8433e-de13-40f2-9a66-b2313ccd972b)

i get root flag 3a4225cc9e85709adda6ef55d6a4f2ca












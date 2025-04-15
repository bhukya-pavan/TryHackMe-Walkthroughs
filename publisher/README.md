
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










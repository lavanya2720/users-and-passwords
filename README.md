1. create users.sh
2. vi users.sh - used for writing the bash script
3. chmod 777 users.sh - to give permissions
4. create users.txt
5. vi users.txt - used for adding user names and group names in the below format :
       username; groupname1,groupname2,groupname3 
6. sudo bash users.sh users.txt - to run the script
output :-
User creation complete. 
Log: /var/log/user_management.log. Passwords: /var/secure/user_passwords.csv
Conclusion:
root@DESKTOP-5GL2502:~# sudo cat /var/log/user_management.log  - for executing and checking

2025-10-05 10:18:05 - Created group light
2025-10-05 10:18:05 - Created group dev
2025-10-05 10:18:05 - Added light to groups: sudo,dev,www-data
2025-10-05 10:18:05 - Set permissions for /home/light
2025-10-05 10:18:05 - Password set for light
2025-10-05 10:18:05 - Created group idimma
2025-10-05 10:18:05 - Added idimma to groups: sudo
2025-10-05 10:18:05 - Set permissions for /home/idimma
2025-10-05 10:18:05 - Password set for idimma
2025-10-05 10:18:05 - Created group mayowa
2025-10-05 10:18:06 - Added mayowa to groups: dev,www-data
2025-10-05 10:18:06 - Set permissions for /home/mayowa
2025-10-05 10:18:06 - Password set for mayowa
2025-10-05 10:18:06 - Script completed

root@DESKTOP-5GL2502:~# sudo cat /var/secure/user_passwords.csv  - for executing and checking
light,BsBh6CkRzi9be4
idimma,S6Em5CceuOVpeZ
mayowa,91YhWoR8VmKQtL

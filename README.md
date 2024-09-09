# Linux-Systems-Administration

Ensure/Double Check Permissions on Sensitive Files

Permissions on /etc/shadow should allow only root read and write access.

Command to inspect permissions:
ls -l

![image](https://github.com/user-attachments/assets/67f74d11-c6fa-489c-a001-dfce8af0829b)

Command to set permissions (if needed): sudo chmod /etc/shadow

![image](https://github.com/user-attachments/assets/8d48da50-dda1-41fa-ac4e-56eb8369ec3b)

Permissions on /etc/gshadow should allow only root read and write access.

Command to inspect permissions: ls -l /etc/gshadow

Command to set permissions (if needed): sudo chmod 700 /etc/gshadow

Permissions on /etc/group should allow root read and write access, and allow everyone else read access only.

Command to inspect permissions: ls -l /etc/group

Command to set permissions (if needed): sudo chmod 744 /etc/group

Permissions on /etc/passwd should allow root read and write access, and allow everyone else read access only.

Command to inspect permissions: ls -l /etc/passwd

Command to set permissions (if needed): sudo chmod 744 /etc/passwd
![image](https://github.com/user-attachments/assets/31fce8e2-5619-4d3f-a81b-63aa8bca118a)


Step 2: Create User Accounts:

Add user accounts for sam, joe, amy, sara, and admin.

sudo adduser.

Command to add each user account (include all five users).

sudo adduser sam sudo adduser joe sudo adduser amy sudo adduser sara sudo adduser admin
![image](https://github.com/user-attachments/assets/8a4e1d6c-d5a9-4262-83ba-6a84c0fa968e)

Ensure that only the admin has general sudo access. sudo -lU admin1
![image](https://github.com/user-attachments/assets/f58386a1-677f-405a-9112-3feedafc2d47)


Step 3: Create User Group and Collaborative Folder

Add an engineers group to the system.

Command to add group:

sudo addgroup engineers

![image](https://github.com/user-attachments/assets/ad309627-3ffd-4f62-9494-5fdf29c79545)


Add users sam, joe, amy, and sara to the managed group. Command to add users to engineers group (include all four users): sudo usermod -aG sam sudo usermod -aG joe sudo usermod -aG amy sudo usermod -aG sara sudo usermod _aG admin1
![image](https://github.com/user-attachments/assets/0711ebb2-a5dd-433f-a5d6-63b08198fb25)

Create a shared folder for this group at /home/engineers. Command to create the shared folder: sudo mkdir group_sharefolder -p /home/engineer

![image](https://github.com/user-attachments/assets/25c80076-3dbe-4ab8-87a8-2a5a58ed9712)


Change ownership on the new engineers' shared folder to the engineers group. Command to change ownership of engineer's shared folder to engineer group:

sudo chgrp engineers groups_sharefolder
![image](https://github.com/user-attachments/assets/5a1636f2-8629-44e8-b5c2-4539170a3e3c)












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





Command Line Intro:
[Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163056.png)
First, I update, upgrade, and reboot my system to make sure everything is up to date.
![[Pasted image 20251118163241.png]]
I then switch to the root user. The prompt changes to reflect this.
![[Pasted image 20251118163640.png]]
To familiarize myself with the differences between the useradd and adduser commands, I add two new users to the system. The difference between the two commands is that useradd just adds a user, whereas adduser prompts you to give them a password and personal information.
![[Pasted image 20251118163850.png]]
Upon changing to the new user sally, the prompt changes by replacing root with sally and becoming colorful again.
![[Pasted image 20251118163951.png]]
As sally, you cannot add further users since the user lacks permissions for it.
![[Pasted image 20251118164529.png]]
I then go back to my user, and list the users on the PC to check that the user I tried to create as sally doesn't exist, and it doesn't. (passwd is not shown since all the users wouldn't fit in a single screenshot)
![[Pasted image 20251118164714.png]]
I change sally's password to "sally123", which is a fine password if I intend for the user to change it to something else upon logging in, which is why I can ignore the password quality warning.
The rest of my practice will be completed as my main user to build the habit of not staying logged in as root for long periods of time as to avoid a tailgating attack.
![[Pasted image 20251118171401.png]]
I am in the groups users, plugdev, dip, sudo, cdrom, adm, and lhostiuk.
![[Pasted image 20251118172108.png]]
![[Pasted image 20251118172249.png]]
I then gave sally sudo access, and tested her perms by creating a new user.
![[Pasted image 20251118172517.png]]
To familiarize myself with groups, I added a new group, added sally to it, then checked to see if she was added correctly.
![[Pasted image 20251118172818.png]]
I added a new directory, lab1, and checked the perms. I am the owner and group owner of the directory, and the group and I can read write and execute files from the directory, while other users can only read and execute them.
![[Pasted image 20251118173457.png]]
I then made my first bash script, a simple hello world.
![[Pasted image 20251118173624.png]]
It has the permissions for myself and my group to read write and execute, while other users can only read or execute it.
![[Pasted image 20251118174248.png]]
I then checked the ACL and gave sally specific permissions to read and execute the file.
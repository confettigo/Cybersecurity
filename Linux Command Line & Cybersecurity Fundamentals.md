### Command Line Intro:
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163056.png?raw=true)
<br>First, I update, upgrade, and reboot my system to make sure everything is up to date.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163241.png?raw=true)
<br> I then switch to the root user. The prompt changes to reflect this.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163640.png?raw=true)
<br> To familiarize myself with the differences between the useradd and adduser commands, I add two new users to the system. The difference between the two commands is that useradd just adds a user, whereas adduser prompts you to give them a password and personal information.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163850.png?raw=true)
<br> Upon changing to the new user sally, the prompt changes by replacing root with sally and becoming colorful again.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118163951.png?raw=true) 
<br> As sally, I cannot add further users since the user lacks permissions for it.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118164529.png?raw=true)
<br> I then go back to my user, and list the users on the PC to check that the user I tried to create as sally doesn't exist, and it doesn't. (passwd is not shown since all the users wouldn't fit in a single screenshot)
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118164714.png?raw=true)
<br> I change sally's password to "sally123", which is a fine password if I intend for the user to change it to something else upon logging in, which is why I can ignore the password quality warning.
The rest of my practice will be completed as my main user to build the habit of not staying logged in as root for long periods of time as to avoid a tailgating attack.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118171401.png?raw=true)
<br> I am in the groups users, plugdev, dip, sudo, cdrom, adm, and lhostiuk.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118172108.png?raw=true)
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118172249.png?raw=true)
<br> I then gave sally sudo access, and tested her perms by creating a new user.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118172517.png?raw=true)
<br> To familiarize myself with groups, I added a new group, added sally to it, then checked to see if she was added correctly.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118172818.png?raw=true)
<br> I added a new directory, lab1, and checked the perms. I am the owner and group owner of the directory, and the group and I can read write and execute files from the directory, while other users can only read and execute them.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118173457.png?raw=true)
<br> I then made my first bash script, a simple hello world.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118173624.png?raw=true)
<br> It has the permissions for myself and my group to read write and execute, while other users can only read or execute it.
![Image](https://github.com/confettigo/Cybersecurity/blob/master/Pasted%20image%2020251118174248.png?raw=true)
<br> I then checked the ACL and gave sally specific permissions to read and execute the file.
# roger-skyline

**V.2  VM Part**
=====================
***
**V.3  Network and Security Part**
=====================
***
• You must create a non-root user to connect to the machine and work.
-----------------------------------
***
None-root user was created while setting-up Debian. Just log in.
***
• Use sudo, with this user, to be able to perform operation requiring special rights.
-----------------------------------
***
First we need to install sudo. So, go to root mode -> update all -> install sudo and vim (optional)
```
$ su 
$ apt-get update -y && apt-get upgrade -y
$ apt-get install sudo vim -y
```
exit from root mode:
```
exit
```
But our not-root user pmelodi isn't in sudoers file!!!
I did following in root mode:
Go to ```/etc``` directory -> add writing mode to ```sudoers``` file -> open it in vim to rewrite
![alt text](screenshots/add_user_sudo0.png) --> ![alt text](screenshots/add_user_sudo1.png)

We don’t want you to use the DHCP service of your machine. You’ve got to configure it to have a static IP and a Netmask in \30.
-----------------------------------
**VI.1 Web Part**
=====================
***
**VI.2 Deployment Part**
=====================
***

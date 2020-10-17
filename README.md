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

• We don’t want you to use the DHCP service of your machine. You’ve got to configure it to have a static IP and a Netmask in \30.
-----------------------------------
The Dynamic Host Configuration Protocol (DHCP) is a network management protocol used on Internet Protocol (IP) networks, whereby a DHCP server dynamically assigns an IP address and other network configuration parameters to each device on the network, so they can communicate with other IP networks.
DHCP (Dynamic Host Configuration Protocol — протокол динамической настройки узла) — сетевой протокол, позволяющий сетевым устройствам автоматически получать IP-адрес и другие параметры, необходимые для работы в сети TCP/IP. Данный протокол работает по модели «клиент-сервер».
**VI.1 Web Part**
=====================
***
**VI.2 Deployment Part**
=====================
***

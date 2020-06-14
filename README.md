# WSL_SSH_Scripts

![SSH](https://www.razoyo.com/wp-content/uploads/2018/12/ssh.jpg)

https://docs.microsoft.com/en-us/wind...

https://www.digitalocean.com/communit...

sudo apt-get update

sudo apt install openssh-server

sudo ssh-keygen -A

sudo nano /etc/ssh/sshd_config

CHANGE

PermitRootLogin prohibit-password to PermitRootLogin yes 
PasswordAuthentication no to PasswordAuthentication yes

sudo service ssh --full-restart

ssh username@192.168.0.X

whoami

ifconfig | grep '192.168.0.' | awk '{print $2}' | tr -d 'addr:';


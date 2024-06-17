# linux-herk
Su

Root

Zipper search samba kan ook zypper install samba

Maak screenshot van uitslag



Systemctl start smb.service

Systemctl status smb.service

Screenshot





Apache

Zypper install apache2

Maak screenshot

Systemctl start apache2.service

Systemctl status apache2.service

Maak screenshot

Cd /srv/www/

Ls zoek naar vhsost anders maak aan

Mkdir vhosts

Cd vhosts/

Mkdir nederland.local england.local

Vi nederland.local/index.html

Dit is nl website 

Opslaan

Doe het zelfde met engeland.local

Tree 

Maak screenshot

Ip address

Kopier de ip address

Vi /etc/hosts

Voeg ip toe en nederland.host

Maak screen shot

Cd /etch/apache2/vhost.d/

Cp vhost.templete nederland.conf doe bij engeland ook

Ls

Screenshot

Vi engeland.conf

:1,$ s/dummy-host.example.com/england.local/g

En does bij nederland ook

Mag screenshot maken

Systemctl restart apache2.service

Stop firewalld.service

Maak screenshot van allebei website

In windows 

Ipadress/nederland.local



Samba

Su

Root

Cd /home

Ls

Mkdir share1 share2

Ls

Screenshot

Vi /etc/samba/smb.conf



[share1]

Path = /home/share1

Writable = yes



[share2]

Path = /home/share2

Writable = yes



Ex

Useradd user1

Useradd user2

Passwd user 1

Passwd user 2

Smb passwd -a user1

Smb passwd -a user2

Screenshot



Groupadd groep a

Groupadd groep b

Usermode -g groep a user1

Usermode -g groep b user2

Id user 1 

Id user2

Maak screenshot

Chgrp groepa share1



Chgrp groepb share2

Chmod 770 share 1

Chmod 770 share2

Ls -l 

Screenshot

Systemctl restart smb.service

Ip adress

Firwwall stop

Naar windows client

Log in via verkenner

Maak screenshot van credantial

Maak screenshot dat je erin zit

Disconnect met de oude share voordat beginnen met nieuwe share



Ls -l









Office instaleren en screenshot maken









Su 

Root











Linux 2





Zypper install clamav

Screenshot

Freshclam

Screenshot



Clamscan /home/share1

screen shot

Clamscan /home/share2

Screenshot

Clanscan /home

Screenshot





Backup

Cd /tmp

Mkdir backup

Ls 

Cd /home

Vi backup.sh

#!/bin/bash



Rsynch -av /home/share1 /tmp/backup

Rsynch -av /home/share2 /tmp/backup

Rsynch -av /home /tmp/backup

Opslaan

Cat backup.sh

Screenshot

Chmod +x backup.sh

Screenshot

./backup.sh

Screenshot

Ls /tmp/backup/

Screenshot

Crontab -e

0 0 * * * /home/backup.sh

Crontab -l 

Screenshot



Linux 2 testrapport



Linux 2 testrapport

Testrapport

Setfacl -m g:groepa:r-x share2

Setfacl -m g:groepb:r-x share1

Screenshot

Credential screenshot

Op wie je inlog voor testen

Probeer nieuw bestand aanmaken en maak screenshot



Systemctl start smb.servicd

Systemctl enable nmb.service 





Lan speed test

\\ipadress\share1


Elke share moet je aanmelden met de juiste gebruiker

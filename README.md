# Linux-Scripting
Scripting for Servers

yeremy@yeru:~$ vi useradd.sh
#!/bin/bash

for i in $(cat /home/yeremy/UserNamesLvl1.txt ); do
    useradd $i
     echo "Welcome $i !"
      echo "password" | chpasswd
       echo " Password has been created for $i  !"
done

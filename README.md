# Autoinstall Eclipse on Ubuntu and MacOS #

This script, eclipse-installer, will install the Eclipse SDK with PHP, Python, C++, 
Ruby, and ShellEd on Ubuntu and MacOS. It will also setup the Eclipse 
launch script to move Oracle 8 Java JDK to the /run/shm RAM Disk for 
Ubuntu only.

To install new or different versions of Eclipse change the eclipserel and 
eclipserelver variables to match the target version.

This script will delete the previous version of Eclipse including the eclipse.ini. 
It will rebuild the eclipse.ini via the script. 

## Ubuntu eclipse.ini ##
```
-XX:+AggressiveOpts
-XX:PermSize=512m
-XX:MaxPermSize=512m
-Xms2048m
-Xmx2048m
-Xmn512m
-Xss2m
```
## MacOS eclipse.ini ##
```
-XX:+AggressiveOpts
-XX:PermSize=512m
-XX:MaxPermSize=512m
-Xms2048m
-Xmx2048m
-Xmn512m
-Xss2m
```

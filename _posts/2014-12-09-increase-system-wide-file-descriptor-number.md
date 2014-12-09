---
layout: post
title: To set a system wide limit for open files on Ubuntu Linux
---


1. Find the current maximum number of open files per user in a single session:
ulimit -n

By default the number is 1024 which is too small.

2. Edit the limits.conf file:
sudo gedit /etc/security/limits.conf
Add the following lines to the file:

   * soft nofile 10000 
   * hard nofile 50000

This sets for all users a soft limit of 10000 open files and a hard limit of 50000. 
These are just example numbers. Set them according to your system needs. Note that the wildcard option applies only to regular users, not to superuser.

Save the file.

3. Edit the configuration file for session-related modules:

sudo gedit /etc/pam.d/common-session
Add the following line to the file:
session required pam_limits.so
Save the file.

4. Restart Ubuntu.

Verify the new maximum number of open files:
ulimit -n 

It is tested on Ubuntu 14.04.

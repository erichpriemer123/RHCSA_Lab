After learning about user management for the RHCSA exam, I believe it is in my best interest to learn how to properly setup Identity management, to avoid the pain that is 
configuring users/groups accross a fleet of servers.
What I have learned about users and groups from chapter 5/6: 
- 5 files for user/group management= passwd, shadow, group, gshadow, login.defs
- There are many commands that let you make changes to these files.
  - groupadd,groupmod,groupdel  =  basic group config commands
  - useradd,usermod,userdel   =  basic user config commands
  - passwd,chge  =  password/password aging commands, lock/unlock user accounts
  - last,lastb,lastlog  =  login history
  - who, w =  currently logged in users. consults udevd
- We can allow users root privleges using the sudoers file. Sudoers file can be changed using visudo.

While this is all wonderful information, this have been the most boring part of my studies so far. So to reinforce my understanding of user/group management,
I will setup red hat identity management using ansible. This should improve my overall understanding of what it means to manage users and groups for multiple servers,
rather than memorize user management commands, as well as improve my understanding of ansible. 
 

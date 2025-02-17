Was having trouble understanding set GID bit on directories. The book was saying if I set gid bit on a directory, any file then created in that directory would become owned by the group, 
allowing for shared read/write/execute on those files. This is only a half truth. While those files created are owned by the group with the set gid bit on the directory, they take on the permissions as decribed 
by the users umask. A suitable umask must be used in order to have a true collabrative directory. 

This was discovered by testing. The book does go into detail on the umask.

Resource : 
  https://serverfault.com/questions/93894/whats-the-purpose-of-setgid-directory#:~:text=Yes%20you%20are%20right%2C%20other,directory%2C%20this%20limited%20its%20use.



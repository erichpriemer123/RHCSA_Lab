find files : 

find command to search for all files in the entire directory structure that have been modified in the last 300 minutes and displays there type.
Using man  files this is what I was able to come up with : 

- find / -mmin -300 -exec file '{}' \;

search for named pipe and socket files:

- find / -type p,s -exec file '{}' \;


summary : google isnt neccassary when you have man pages and a dream

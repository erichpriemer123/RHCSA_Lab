As root, use find to search for regular files under the /usr that were accessed more than 100 days ago, are not bigger than 5MB in size, and are owned by the root user.

answer :
- find /usr -atime +100 -size -5M -type f -user root

---
Tags: # 标签数量丰俭由人
  - Linux
TocOpen: true
author:
  - boz
comments: true
cover:
  alt: ''
  caption: ''
  image: 'posts/cover.jpg'
  relative: true
date: '2025-03-14'
description: '' # 为页头简介，省略
disableShare: true
draft: false # 未发布时为 true
hidemeta: false
lastmod: '2025-03-14'
showToc: true
showbreadcrumbs: true
slug: ''
title: Linux Find Command Examples
weight: null # 若置顶则为对应数字
---


## 1. Find Files by Name
```Linux
find /home/user/documents -name "example.txt"
```
## 2. Find Files by Extension
```Linux
find /var/log -name "*.log"
```
## 3. Find Files modified in the last 7 days
```Linux
find /etc -mtime -7
```
## 4. find files modified more than 30 days ago
```Linux
find /usr/local -mtime +30
```
## 5. Find and delete files
```Linux
find /tmp -name "oldfile.txt" -delete
```
## 6. Find empty files or directories
```Linux
find /var/www/ -empty
```
## 7. Find files larger than 100MB
```Linux
find /home/user/downloads -size +100MB
```
## 8. Find files owned by a specific user
```Linux
find /home -user username
```
## 9. Find files with 0644 permissions
```Linux
find /etc/-perm 0644
```
## 10. Find files and execute a command (gzip log files)
```Linux
find /var/log -name "*.log" -exec gzip {} \;
```
## 11. Find files and execute a command (delete empty files)
```Linux
find /home/user/documents -type f -empty -exec rm {} \;
```
## 12. Find files and print their details
```Linux
find /home/user/documents -type f -exec is -lh {} \;
```
## 13. Find files excluding a specific directory
```Linux
find / -path "/proc" -prune -o -name "*.conf"
```
## 14. Find files modified in the last 60 minutes
```Linux
find /var/www -mmin -60
```
## 15. find and archive files with a specific extension
```Linux
-czvf archive.tar.gz
```
## 16. Find symbolic links
```Linux
find /usr/bin -type l
```
## 17. Find files by lnode number
```Linux
find / -inum 456332
```
## 18. Find files and exclude a specific file type
```Linux
find /home/user -not -name "*.txt"
```
## 19. Find files with specific group ownership
```Linux
find /var/log -group syslog
```
## 20. Find files with specific size range (e.g., 500MB to 100MB)
```Linux
find /home/user/downloads -size +50M -size +100MB
```
## 21. Find and sort files by modification time
```Linux
find /var/log -type f exec ls -lt {} +
```
## 22. Find files modified in the last 2 hours
```Linux
find /var/log -mmin -120
```
## 23. Find files with specific user and group ownership
```Linux
find /home -user username -group groupname
```
## 24. Find fils with specific file permissions (readable by owner only)
```Linux
find /var/log -perm 600
```
## 25. Find files larger than 1GB and Delete Them
```Linux
find /var/log -size +1G -exec rm -f {} \;
```
## 26. Find files and limit depth of search to 1 level
```Linux
find /home/user -maxdepth 1 -name "*.txt"
```
## 27. Find files accessed more than 90 days ago
```Linux
find /var/log -atime +90
```
## 28. Find hidden files
```Linux
find /home/user -name ".*"
```
## 29. Find files created more than 1 day ago
```Linux
find /home/user -ctime +1
```
## 30. Find files by their type (e.g., Block Devices)
```Linux
find /dev/ -type b
```
## 31. Find files with specific permission and exclude others
```Linux
find / -perm /a=r -not -perm /a=w
```
## 32. Find files containing a specific string in the name
```Linux
find /home/user -name "*config*"
```

link: sysxplore.com
#  Website backup script

This script allows to backup your site's files and database over SSH. More details on my website : https://ludovicscribe.fr/blog/script-sauvegarde-site-web

## Prerequisites

- You must have an SSH access to your web hosting
- You must have an SSH access to your web hosting
- sshpass must be installed on your computer
- ssmtp and mailutils must be installed and configured on your computer

## Configuration

If you want, you can rename the mysite.config file to your site's name. Then, you have to edit it and fill some parameters :
- Project name
- Notification email address
- SSH  : host, login and password
- MySQL : host, login, password and database name
- Remote and local directories

## Execution

To execute the script, you must pass it the config file's path :
```
./backup-site.sh /home/pi/mysite.config
```

Your backup will be stored in the directory specified in the "LOCAL_DIR" parameter, categorized by project and month.
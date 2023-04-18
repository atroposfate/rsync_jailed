# Rsync Jail Setup
Build a Chroot jail for a user that is backing files up

This is a rookie setup script that creates the files needed for the jail to run rysnc and some simple 'ls' to review issues

The intention is on the remote server a cronjob is running as root to back-up the /etc/ folder or whatever other area you want to back up and save it to this users home directory. Important that the root user is updating the ownership to the same user that will be running rsync and the backup server will pull the folder that the backup was saved to

This script solved the problem of having a privlaged user having remote access to the server. This user can only log into a jail and download the backups

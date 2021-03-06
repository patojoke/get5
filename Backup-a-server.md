# DISCLAIMER
Please note the below procedure assumes you have been using csgosl in the standard way, i.e. no manual
editing of config files or manually installed own source mod plugins, ... If you have done this the below procedure will describe how to restore your server but you will have to backup and reapply all your manual changes yourself.

# UPDATE
I completely forgot about workshop maps. They will be lost with the method described below. I currently don't have time to test this out but maybe all you need to do is copy the workshop maps as well into the backup and restore them? If so, that's a simple workaround for now. I will look into how to automatically redownload the workshop maps.

# General
The below procedure will describe how to make a complete but small backup of your server installation. In my test case the entire installation was 16.3GB and the backup was 0.1GB.

# Assumptions
Your source server is installed in <some-path>/csgosl. The source server is the one you want to backup.
Your backup will be stored in <backup-path>/csgosl. This folder will only contain what is necessary to backup, not the complete installation.
The target server will be installed in <some-other-path>/csgosl. The target server is the server you restore from the backup.

# Example paths
linux:<br>
Your user name: nisse<br>
`Source path: /home/nisse/csgosl`<br>
`Backup path: /home/nisse/csgosl-backup`<br>
`Restore path: /home/nisse/csgosl-restore`<br>
<br>
windows:<br>
`Source path: c:\csgosl`<br>
`Backup path: c:\csgosl-backup`<br>
`Restore path: c:\csgosl-restore`<br>

# Backup procedure
1. Copy source path folder contents excluding folders `server` and `steamcmd` to backup folder.
1. Done!

Windows example:
Browse to your source folder and select all files except the folders mentioned above. (c:\csgosl in the example)

![Select backup source](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/backup-select-source.jpg)

Paste the files into the backup folder (c:\csgosl-backup in the example)

![Paste into backup folder](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/backup-paste-backup-folder.jpg)

# Restore procedure
1. Copy backup folder contents to target folder.
1. Start server in target folder. csgosl will now reinstall the server files from Valve keeping all your settings.
1. Done!

Browse to your backup folder and select all files. (c:\csgosl-backup in the example)

![Select backup folder](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/backup-folder.jpg)

Paste the files into the backup restore folder (c:\csgosl-restore in the example)

Start the server as you usually do by clicking one of the selected files below.
![Select backup folder](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/backup-start-server.jpg)

Your server is now reinstalled keeping all your settings.
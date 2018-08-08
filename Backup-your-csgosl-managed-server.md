# DISCLAIMER
Please note the below procedure assumes you have been using csgosl in the standard way, i.e. no manual
editing of config files or manually installed own source mod plugins, ... If you have done this the below procedure will describe how to restore your server but you will have to reapply all your manual changes yourself.

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
1. Copy source path folder excluding folders `server` and `steamcmd` to backup folder.

# Restore procedure
1. Copy backup folder to target folder.
1. Start server in target folder. csgosl will now reinstall the server files from Valve keeping all your settings.

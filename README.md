# Default Vagrant box for Anyforsoft projects

## Vagrant installation
1. Check/install NFS to your system https://help.ubuntu.com/community/SettingUpNFSHowTo
2. Copy ./vagrant directory to you project
3. Run "cd vagrant" in project docroot
4. Run "vagrant up"
5. On http://192.168.33.10 you should see empty apache page site
6. To use ssh, phing, drush sync you can copy your ssh key to virtual machine

## Other useful features

* "vagrant --help" - all vagrant commands
* "vagrant ssh" - vagrant machine access
* "error" - apache error logs
* "web" - apache site folder

## Mailcatcher

1. "mailcatcher --http-ip=0.0.0.0" - start mailcatcher
2. Visit http://192.168.33.10:1080 to see mailcatcher page

## Xdebug

To configure remote xdebug see *.png

## MySQL

* Database access:
* User: root
* Password: root
* Database: site

## Windows users

You can have error that vagrant installed Guest Additions, needs restart guest system and he can't mount folder.

It is OK you need just to run "vagrant reload" and then "vagrant provision" to run startup scripts again.

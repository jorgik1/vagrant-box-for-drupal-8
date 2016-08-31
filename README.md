# Default Vagrant box for Anyforsoft projects

## Vagrant installation
1. Copy ./vagrant directory to you project
2. Run "cd vagrant" in project docroot
3. Run "vagrant up"
4. On http://192.168.33.10 you should see empty apache page site

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

create a user with the adduser command.

## Task

This command will create a user account. Change new_user to any name you like!
try and type each command yourself.  These commands come in handy all the time.

* create your user account `sudo adduser new_user`{{execute}}
* Username add here, type `new_user`{{execute}}
* enter data if you want, type `NA`{{execute}}
* enter data if you want, type `NA`{{execute}}
* enter data if you want, type `NA`{{execute}}
* enter data if you want, type `NA`{{execute}}
* Confirm everything is correct and hit Yes, type `Y`{{execute}}
* Here we list all users and see our user was added, type `sudo awk -F: '{ print $1}' /etc/passwd`{{execute}}

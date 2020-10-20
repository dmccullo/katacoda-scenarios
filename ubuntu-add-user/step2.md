create a user with the adduser command.

## Task

No that we have a user we will login with that user, create an ssh key pair and configure the account to use that keypair.

try and type each command yourself.  These commands come in handy all the time.

* SUDO to the user account we created, type `sudo su - new_user`{{execute}}
* create an SSH Key Pair (you can do htis locally and create your .pub key here by editing it and copying and pasting the contents to a local file if you like, type `ssh-keygen -t rsa -m PEM  -C user@domain.com `{{execute}} 

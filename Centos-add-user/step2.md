Login to the new user account and create their SSH key pair and configure the account to use it.

## Task

Now that we have a user we will login with that user, create an SSHkey pair and configure the account to use that keypair.

try and type each command yourself.  These commands come in handy all the time.

* Sudo to the user account we created, type `sudo su - new_user`{{execute}}
* change to new_user's home directory, type `cd ~/`{{execute}}
* create an SSH Key Pair (you can do this locally and create your .pub key here by editing it and copying and pasting the contents to a local file if you like, type * * Enter this command to create a User SSH key, type `ssh-keygen -t rsa -m PEM  -C new_user@new-user.com`{{execute}}
* Name your key, type `new_user-key`{{execute}}
* If you like add a Pin so your private key cannot be used by anyone but you, type `12345`{{execute}}
* Confirm your pin, type `12345`{{execute}}
* let's see our Key Pair, type `ls -la`{{execute}}
We are almost done a couple more step to allow the user to login.
Next we need to create a directory and create a file in it.
* make the users .ssh directory, type `mkdir .ssh`{{execute}}
* Update permissions on the directory, type `chmod 700 .ssh`{{execute}}
* create the authorized_keys file the SSH service needs, type `touch .ssh/authorized_keys`{{execute}}
* change permissions on the Authorized_Keys file, type `chmod 600 .ssh/authorized_keys`{{execute}}
* add your key to the authorized_keys file, type `cat new_user-key.pub >> .ssh/authorized_keys`{{execute}}

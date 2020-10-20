Login to the new user account and create their SSH key pair and configure the account to use it.

## Task

Now that we have a user we will login with that user, create an SSHkey pair and configure the account to use that keypair.

try and type each command yourself.  These commands come in handy all the time.

* Sudo to the user account we created, type `sudo su - new_user`{{execute}}
* change to new_user's home directory, type `cd ~/`{{execute}}
* create an SSH Key Pair (you can do htis locally and create your .pub key here by editing it and copying and pasting the contents to a local file if you like, type * * Enter this command to create a User SSH key, type `ssh-keygen -t rsa -m PEM  -C new_user@new-user.com`{{execute}}
* let's see our Key Pair, type `ls -la` {{execute}}

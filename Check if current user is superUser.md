Run `sudo -v`. It is usually used to extend your sudo password timeout, but can be used for determining whether you have any sudo privileges.
```
$ sudo -v
Sorry, user [username] may not run sudo on [hostname].
```

Man page excerpt:

If given the -v (validate) option, sudo will update the user’s time stamp, prompting for the user’s password if necessary. This extends the sudo timeout for another 5 minutes (or whatever the timeout is set to in sudoers) but does not run a command.

If your user is only allowed to run specific commands, this command will work, indicating you are allowed to run something with different privileges. While the message looks different when trying to execute a command you're not allowed to in this case (and no mail is sent to root), it's still possible you'll get into trouble if the admins read /var/log/secure.

```
$ sudo ls
[sudo] password for [username]: 
Sorry, user [username] is not allowed to execute '/bin/ls' as root on [hostname].
```
To find out what you're allowed to run with different privileges, you can use sudo -l. Note that this command requires you to enter your password.

### Swith to root:
```
          $ sudo -i
```
 Enter password for current user when prompted
```
            [sudo] password for <currentUser>: 
```
### Verify root access:
Method 1:
```
             root@ubuntu:~# id
             uid=0(root) gid=0(root) groups=0(root)
```
Method 2:
```
              root@ubuntu:~# whoami
              root
```

NOTE : Notice symbol `$` has changed to `#`

### Exit root:
```
              exit
```
OR
```
              logout
```

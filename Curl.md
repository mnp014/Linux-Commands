#### Ubuntu install curl command
First update the system and get latest stable curl version for Ubuntu:
```
          $ sudo apt update
          $ sudo apt upgrade
```
Type the following apt command or apt-get command:
```
          $ sudo apt install curl
```

#### Verification
Run the following command:
```
        $ curl --version
```

#### Usage
Once installed you can use it as follows to see the headers:
```
        $ curl -I https://www.google.com/
```

Or download a file from a server using curl itself:
```
        $ curl -o output.file http://server1.abc.com/page1.foo.txt
```
You can resume broken download with the curl command as follows:
```
        $ curl -L -O -C - http://ftp.ussg.iu.edu/linux/centos/latest/isos/file.iso
```


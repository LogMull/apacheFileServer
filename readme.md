# File Server
Basic file server for accessing stuff outside of the home

Assumed that a directory is mounted at /mnt/cerebro

Access should be controlled by Authelia via caddy.

``` sh
# sudo mount -t cifs //192.168.4.10/mnt/user/FileSharing /mnt/cerebro -o username=apache,password=Perpetual2-Cinch-Carbon,vers=3.0
```

Or in fstab
```sh
192.168.4.10:/mnt/user/FileSharing  /mnt/cerebro  nfs  nolock,sec=sys,vers=3  0  0
```
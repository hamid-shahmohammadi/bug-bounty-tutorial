# bug-bounty-tutorial
bug bounty tutorial

## 23.Discovering-Endpoints-&-Sensitive-Data
```
sudo apt update
sudo apt install -y feroxbuster
feroxbuster --help
feroxbuster -u url -w worldlist
https://github.com/danielmiessler/SecLists/blob/master/Discovery/Web-Content/common.txt
feroxbuster -u http://127.0.0.1:42001/ -w common.xt -o result.txt
```

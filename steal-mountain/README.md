Steal Mountain
Padsala Tushal
14 Aug 2022 | 10:01 AM

10.10.185.79


## Introduction

> Who is the employee of the month?

	port 80 : image -> employee name
```
Bill Harper
```

## Initial Access

>Scan the machine with nmap. What is the other port running a web server on?
```
8080
```

> Take a look at the other web server. What file server is running?
```
Rejetto HTTP File Server
```

> What is the CVE number to exploit this file server?
```
2014-6287
```
> Use Metasploit to get an initial shell. What is the user flag?
```

```

port 8080 : file server
		-with nmap 
			 Rejetto Http File Server 
		-exploit db
		-metasploit


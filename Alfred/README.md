Alfred
Padsala Tushal
14 Aug 2022 | 11:12 am

## Initial Access
> How many ports are open? (TCP only)
```
3
```

> What is the username and password for the log in panel(in the format username:password)

```
admin:admin
```

>What is the user.txt flag? 
```
79007a09481963edf2e1321abd9ae2a0
```

## Switching Shell

>What is the final size of the exe payload that you generated?
```
73802
```

## Privilege Escalation


>To check which tokens are available, enter the list_tokens -g. We can see that the BUILTIN\Administrators token is available. Use the impersonate_token "BUILTIN\Administrators" command to impersonate the Administrators token. What is the output when you run the getuid command?

```
NT AUTHORITY\SYSTEM
```

>read the root.txt file at C:\Windows\System32\config
```
dff0f748678f280250f25a45b8046b4a
```
# Anonymous
> Padsala Tushal | 19 Nov 20211
> IP = 10.10.26.17

## Reconnaissance
*nmap*
	-port 21 ftp 
		anonymous login found
	-port 22 ssh
	-port 139 and 445
	-connect to smb
	-found 2 pics in smb
		-corgo2.jpg
		-puppos.jpeg
	-nothing useful in this img

*ftp*
	-we have ftp access and we saw that there is a clean.sh script on ftp 
	-let's replace that clean.sh script and upload our malicious scripts

|User Flag| = 90d6f992585815ff991e68748c414740

## Privilege Escalation

-after get access
-get tty shell
-find suid bit binery
-/usr/bin/env
-gtfo bins

|Root Flag| = 4d930091c31a622a7ed10f27999af363
pickle rick
padsala trushal
24 oct 2021

10.10.116.165

-view source code
	username:R1ckRul3s
-robots.txt
	Wubbalubbadubdub

-find login page 
	login.php
	username:R1ckRul3s
	password:Wubbalubbadubdub


-found command panel
	ls:
		Sup3rS3cretPickl3Ingred.txt
		assets
		clue.txt
		denied.php
		index.html
		login.php
		portal.php
		robots.txt




	-http://10.10.116.165/clue.txt
		Look around the file system for the other ingredient.


	-<!-- Vm1wR1UxTnRWa2RUV0d4VFlrZFNjRlV3V2t0alJsWnlWbXQwVkUxV1duaFZNakExVkcxS1NHVkliRmhoTVhCb1ZsWmFWMVpWTVVWaGVqQT0== -->

-found first flag 
	after acessing command panel file found 
		-http://10.10.116.165/Sup3rS3cretPickl3Ingred.txt
		flag :: mr. meeseek hair

-found second flag
	after looking in file system 
	-less  /home/rick/"second ingredients"
	    note: in less command file name must be in "" other wise linux system can't understand
	flag :: 1 jerry tear

-found third flag
	after looking privileage of user the user run all command with sudo permission
	-sudo less /root/"3rd.txt"
	3rd ingredients: fleeb juice

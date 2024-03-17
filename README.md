
# RootMe | TryHackMe CTF

## Information about target : 
**Url room** : https://tryhackme.com/room/rrootme

**Target IP address** : 10.10.104.61


## Reconnaissance
**Scan the machine, how many ports are open?** : 2

_commande_ :
```bash
nmap -sV 10.10.104.61
```

**What version of Apache is running?** : 2.4.29

**What service is running on port 22?** : ssh

**Find directories on the web server using the GoBuster tool.**

_commande_ :
```bash
gobuster dir -e -u http://10.10.104.61/ -w Downloads/common.txt
```

**What is the hidden directory?** : /panel/
## Getting a shell

**user.txt** : THM{y0u_g0t_a_sh3ll}

[PHP reverse shell script](https://github.com/pentestmonkey/php-reverse-shell/blob/master/php-reverse-shell.php)


## Privilege escalation

**Search for files with SUID permission, which file is weird?** : /usr/bin/python

**root.txt** : THM{pr1v1l3g3_3sc4l4t10n}


## Authors

- [@Rakulan](https://www.github.com/octokatherine)
- [@Roslan]()

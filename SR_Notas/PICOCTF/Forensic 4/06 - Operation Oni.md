
Download this disk image, find the key and log into the remote machine.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download disk image](https://artifacts.picoctf.net/c/70/disk.img.gz)
- Remote machine: `ssh -i key_file -p 56623 ctf-player@saturn.picoctf.net`


(None)


**Solución 1**

```
Ir a la carpeta /tmp

┌──(kali㉿kali)-[/tmp]
└─$ wget https://artifacts.picoctf.net/c/70/disk.img.gz


┌──(kali㉿kali)-[/tmp]
└─$ gzip -d disk.img.gz 

┌──(kali㉿kali)-[/tmp]
└─$ icat disk.img -o 206848 2345 > key_file 


┌──(kali㉿kali)-[/tmp]
└─$ chmod 600 key_file 


┌──(kali㉿kali)-[/tmp]
└─$ ssh -i key_file -p 57728 ctf-player@saturn.picoctf.net

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

ctf-player@challenge:~$ cat flag.txt 
picoCTF{k3y_5l3u7h_b5066e83}ctf-player@challenge:~$ 

```


## Respuesta: **picoCTF{k3y_5l3u7h_b5066e83}**
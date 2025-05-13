
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/138/disk.flag.img.gz)

(None)


**Solución 1**

```
┌──(kali㉿kali)-[~/forensic/forensic4/sleuthkit_apprentice]
└─$ mkdir /tmp/...sleuthkit/                   
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4/sleuthkit_apprentice]
└─$ cd /tmp/...sleuthkit   
                                                                                                          
┌──(kali㉿kali)-[/tmp/...sleuthkit]
└─$ ls
                                                                                                          
┌──(kali㉿kali)-[/tmp/...sleuthkit]
└─$ wget https://artifacts.picoctf.net/c/138/disk.flag.img.gz
--2025-05-07 21:12:57--  https://artifacts.picoctf.net/c/138/disk.flag.img.gz
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 13.225.222.125, 13.225.222.28, 13.225.222.120, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|13.225.222.125|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 47534528 (45M) [application/octet-stream]
Saving to: ‘disk.flag.img.gz’

disk.flag.img.gz           100%[======================================>]  45.33M  2.85MB/s    in 15s     

2025-05-07 21:13:17 (3.08 MB/s) - ‘disk.flag.img.gz’ saved [47534528/47534528]

                                                                                                          
┌──(kali㉿kali)-[/tmp/...sleuthkit]
└─$ gunzip disk.flag.img.gz 

┌──(kali㉿kali)-[/tmp/...sleuthkit]
└─$ icat -f ext4 -o 360448 disk.flag.img 2371
picoCTF{by73_5urf3r_2f22df38}


```



## Respuesta: **picoCTF{by73_5urf3r_2f22df38}**
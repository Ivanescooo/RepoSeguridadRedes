
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/213/disk.flag.img.gz)


(None)


**Solución 1**

```
──(kali㉿kali)-[~/forensic/forensic4/operation_orchid]
└─$ gunzip disk.flag.img.gz 
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4/operation_orchid]
└─$ cd /tmp             
                                                                                                          
┌──(kali㉿kali)-[/tmp]
└─$ ls
config-err-SLcT3s
ssh-XmA3ijl0AW4U
systemd-private-26774b2a20834bc6b88ef345fe43f96c-colord.service-hEy3h1
systemd-private-26774b2a20834bc6b88ef345fe43f96c-haveged.service-rI7vuS
systemd-private-26774b2a20834bc6b88ef345fe43f96c-ModemManager.service-XZjokl
systemd-private-26774b2a20834bc6b88ef345fe43f96c-polkit.service-mDQysk
systemd-private-26774b2a20834bc6b88ef345fe43f96c-systemd-logind.service-l1b3G5
systemd-private-26774b2a20834bc6b88ef345fe43f96c-upower.service-MyS7zr
Temp-e0d0ca5b-d49e-4fe0-a5fb-7351b06e0362
                                                                                                          
┌──(kali㉿kali)-[/tmp]
└─$ mkdir foo             
                                                                                                          
┌──(kali㉿kali)-[/tmp]
└─$ cd     
                                                                                                          
┌──(kali㉿kali)-[~]
└─$ cd forensic/forensic4                       
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4]
└─$ ls
concat_v.png             operation_orchid  ruby-3.4.3.tar.gz  sleuthkit_apprentice
_concat_v.png.extracted  ruby-3.4.3        sleuthkit
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4]
└─$ cd operation_orchid                         
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4/operation_orchid]
└─$ ls
disk.flag.img
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4/operation_orchid]
└─$ sudo mount disk.flag.img /tmp/foo -o offset=$((411648*512))
[sudo] password for kali: 
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic4/operation_orchid]
└─$ cd /tmp/foo  

┌──(kali㉿kali)-[/tmp/foo]
└─$ sudo su

──(root㉿kali)-[~]
└─# cd /tmp/foo/root 
                                                                                                          
┌──(root㉿kali)-[/tmp/foo/root]
└─# openssl aes256 -d -in flag.txt.enc -out decrypt.txt
enter AES-256-CBC decryption password:
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
bad decrypt
40A7E41DFA7F0000:error:1C800064:Provider routines:ossl_cipher_unpadblock:bad decrypt:../providers/implementations/ciphers/ciphercommon_block.c:107:
                                                                                                          
┌──(root㉿kali)-[/tmp/foo/root]
└─# cat decrypt.txt 
picoCTF{h4un71ng_p457_5113beab} 

```



## Respuesta: **picoCTF{h4un71ng_p457_5113beab} }**
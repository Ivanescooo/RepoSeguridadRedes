
Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/260/flag.png).


(None)


**Solución 1**

```
                                                                                                         
┌──(kali㉿kali)-[~/forensic/tarea-forensic/hideme]
└─$ binwalk -e flag.png           

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
41            0x29            Zlib compressed data, compressed
39739         0x9B3B          Zip archive data, at least v1.0 to extract, name: secret/
39804         0x9B7C          Zip archive data, at least v2.0 to extract, compressed size: 2944, uncompressed size: 3095, name: secret/flag.png

WARNING: One or more files failed to extract: either no utility was found or it's unimplemented

                                                                                                          
┌──(kali㉿kali)-[~/forensic/tarea-forensic/hideme]
└─$ ls
flag.png  _flag.png.extracted
                                                                                                          
┌──(kali㉿kali)-[~/forensic/tarea-forensic/hideme]
└─$ cd _flag.png.extracted 
                                                                                                          
┌──(kali㉿kali)-[~/forensic/tarea-forensic/hideme/_flag.png.extracted]
└─$ cd secret             
                                                                                                          
┌──(kali㉿kali)-[~/…/tarea-forensic/hideme/_flag.png.extracted/secret]
└─$ sz flag.png                   
�                

                                                                                                       
┌──(kali㉿kali)-[~/…/tarea-forensic/hideme/_flag.png.extracted/secret]
└─$ eog flag.png 


La bandera sale en la imagen

```



## Respuesta: **picoCTF{Hiddinng_An_imag3_within_@n_ima9e_ad9f6587}**
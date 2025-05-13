
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/a614a27d4cb251d04c7d2f3f3f76a965/cat.jpg)


Hints:
Look at the details of the file.
Make sure to submit the flag as picoCTF{XXXXX}.


**Solución 1**

```
──(kali㉿kali)-[~/forensic/tarea-forensic/information]
└─$ wget https://mercury.picoctf.net/static/a614a27d4cb251d04c7d2f3f3f76a965/cat.jpg


┌──(kali㉿kali)-[~/forensic/tarea-forensic/information]
└─$ exiftool cat.jpg | grep License | sed -e 's/.*: //' | base64 -d
picoCTF{the_m3tadata_1s_modified} 

```



## Respuesta: **picoCTF{the_m3tadata_1s_modified}**

I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/d3dd8cd51524d9fafcccd1b7d55f85e7/Forensics%20is%20fun.pptm)


None



**Solución 1**

```

┌──(kali㉿kali)-[~/forensic/forensic3/MacroHard_WeakEdge]
└─$ unzip Forensics\ is\ fun.pptm -d macro
Archive:  Forensics is fun.pptm

┌──(kali㉿kali)-[~/forensic/forensic3/MacroHard_WeakEdge]
└─$ cd macro                               
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic3/MacroHard_WeakEdge/macro]
└─$ cd ppt 

┌──(kali㉿kali)-[~/…/forensic3/MacroHard_WeakEdge/macro/ppt]
└─$ cd slideMasters 

┌──(kali㉿kali)-[~/…/MacroHard_WeakEdge/macro/ppt/slideMasters]
└─$ cat hidden| sed 's/ //g' | base64 -d                    
flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}


```



## Respuesta: **picoCTF{D1d_u_kn0w_ppts_r_z1p5}**




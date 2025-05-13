
Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/1b70cffdd2f05427fff97d13c496963f/dolls.jpg)

Hints:
Wait, you can hide files inside files? But how do you find them?
Make sure to submit the flag as picoCTF{XXXXX}



**Solución 1**

```

Descargar la imagen

En consola:

-----------------------------------------------------------------------------------

┌──(kali㉿kali)-[~/forensic/forensic3/Matryoshka_doll]
└─$ foremost dolls.jpg
Processing: dolls.jpg
|foundat=base_images/2_c.jpgUT
*|

┌──(kali㉿kali)-[~/forensic/forensic3/Matryoshka_doll]
└─$ ls
dolls.jpg  output
                                                                                                          
┌──(kali㉿kali)-[~/forensic/forensic3/Matryoshka_doll]
└─$ cd output/zip     
                                                                                                          
┌──(kali㉿kali)-[~/…/forensic3/Matryoshka_doll/output/zip]
└─$ ls
00000532.zip
                                                                                                          
┌──(kali㉿kali)-[~/…/forensic3/Matryoshka_doll/output/zip]
└─$ unzip 00000532.zip      
Archive:  00000532.zip
  inflating: base_images/2_c.jpg     
                                                                                                          
┌──(kali㉿kali)-[~/…/forensic3/Matryoshka_doll/output/zip]
└─$ ls
00000532.zip  base_images
                                                                                                          
┌──(kali㉿kali)-[~/…/forensic3/Matryoshka_doll/output/zip]
└─$ cd base_images   
                                                                                                          
┌──(kali㉿kali)-[~/…/Matryoshka_doll/output/zip/base_images]
└─$ foremost 2_c.jpg  
Processing: 2_c.jpg
|foundat=base_images/3_c.jpgUT
*|
                                                                                                          
┌──(kali㉿kali)-[~/…/Matryoshka_doll/output/zip/base_images]
└─$ cd output/zip 
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ ls
00000366.zip
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ unzip 00000366.zip 
Archive:  00000366.zip
  inflating: base_images/3_c.jpg     
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ cd base_images 
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ ls
3_c.jpg
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ foremost 3_c.jpg 
Processing: 3_c.jpg
|foundat=base_images/4_c.jpgUT
*|
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ ls
3_c.jpg  output
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ cd output/zip 
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ ls
00000241.zip
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ unzip 00000241.zip 
Archive:  00000241.zip
  inflating: base_images/4_c.jpg     
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ cd base_images 
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ foremost 4_c.jpg 
Processing: 4_c.jpg
|foundat=flag.txtUT
*|
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ ls            
4_c.jpg  output
                                                                                                          
┌──(kali㉿kali)-[~/…/base_images/output/zip/base_images]
└─$ cd output/zip 
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ ls
00000155.zip
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ unzip 00000155.zip 
Archive:  00000155.zip
  inflating: flag.txt                
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ ls           
00000155.zip  flag.txt
                                                                                                          
┌──(kali㉿kali)-[~/…/zip/base_images/output/zip]
└─$ cat flag.txt   
picoCTF{bf6acf878dcbd752f4721e41b1b1b66b} 

```



## Respuesta: **picoCTF{bf6acf878dcbd752f4721e41b1b1b66b}**




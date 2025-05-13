
Can you get the real meaning from this file.Download the file [here](https://artifacts.picoctf.net/c_titan/108/enc_flag).


Hints:
Engaging in various decoding processes is of utmost importance


**Solución 1**

```
┌──(kali㉿kali)-[~/crypto/interencdec]
└─$ base64 -d enc_flag 
b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2g0N2o2azY5fQ=='
    

En cyberchef:

from base64
entrada: d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2g0N2o2azY5fQ==
salida: wpjvJAM{jhlzhy_k3jy9wa3k_h47j6k69}


en caesar cipher decoder:
ciphertext: wpjvJAM{jhlzhy_k3jy9wa3k_h47j6k69}
se cambia hacia  plaintext: picoCTF{caesar_d3cr9pt3d_a47c6d69}

```


## Respuesta: **picoCTF{caesar_d3cr9pt3d_a47c6d69}**


Link: https://cryptii.com/pipes/caesar-cipher
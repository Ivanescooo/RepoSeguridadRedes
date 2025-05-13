
There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?

There is data encoded somewhere... there might be an online decoder.


**Solución 1**

```

(kali㉿kali)-[~/forensic/forensic1/whatlieswithin]
└─$ zsteg -a buildings.png                                                                             
b1,r,lsb,xy         .. text: "^5>R5YZrG"
b1,rgb,lsb,xy       .. text: "picoCTF{h1d1ng_1n_th3_b1t5}"
b1,abgr,msb,xy      .. file: PGP Secret Sub-key -


```


## Respuesta: **picoCTF{h1d1ng_1n_th3_b1t5}**


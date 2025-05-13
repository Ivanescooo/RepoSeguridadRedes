
The flag is somewhere on this web application not necessarily on the website. Find it.Check [this](http://saturn.picoctf.net:56632/) out.

None


**Solución 1**

```

Agregar a la url "robots.txt"

muestra lo siguiente:
User-agent *
Disallow: /cgi-bin/
Think you have seen your flag or want to keep looking.

ZmxhZzEudHh0;anMvbXlmaW
anMvbXlmaWxlLnR4dA==
svssshjweuiwl;oiho.bsvdaslejg
Disallow: /wp-admin/



Copiar esto: anMvbXlmaWxlLnR4dA==

pasarlo a cyberchef

Input: anMvbXlmaWxlLnR4dA==

Recipe: 
	From Base 64

js/myfile.txt


colocar eso en la url, borrando el robots.txt

y sale la bandera


```


## Respuesta: **picoCTF{Who_D03sN7_L1k5_90B0T5_22ce1f22}**


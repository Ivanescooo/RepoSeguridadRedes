

Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:21939/](http://mercury.picoctf.net:21939/)


Hints:
Maybe you have more than 2 choices

Check out tools like Burpsuite to modify your requests and look at the responses



**Solución 1**

```

Descargar burpsuite y foxyproxy 

interceptar la petición y modificar la parte que dice GET a HEAD, de esta forma la response indica la bandera

presionar boton rojo, interceptar el mensaje obtenido, ver historial y saldrá la bandera

```


## Respuesta: **picoCTF{r3j3ct_th3_du4l1ty_6ef27873}**



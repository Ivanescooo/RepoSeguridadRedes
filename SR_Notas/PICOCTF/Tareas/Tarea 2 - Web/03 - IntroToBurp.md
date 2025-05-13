
Try [here](http://titan.picoctf.net:62196/) to find the flag


Hints:
Try using burpsuite to intercept request to capture the flag.

Try mangling the request, maybe their server-side code doesn't handle malformed requests very well.



**Solución 1**

```

Llenar formulario, dar a register
Dar a forward 2 veces

Escribir el otp en el campo, dar enviar

En la request borrar la última línea que dice OTP="valor ingresado"


```


## Respuesta: **picoCTF{#0TP_Bypvss_SuCc3$S_2e80f1fd}**


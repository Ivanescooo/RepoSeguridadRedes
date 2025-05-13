
A group of underground hackers might be using this legit site to communicate. Use your forensic techniques to uncover their messageTry it [here](http://standard-pizzas.picoctf.net:59520/)!


In the country that doesn't exist, the flag persists


**Solución 1**

```
Abrir la página web, checar cuál país no existe, es "Upanzi", la imagen de ese país es upz.png

en la ruta agregar: /flags/upz.png
descargar la imagen



En consola:

┌──(kali㉿kali)-[~/forensic/tarea-forensic/flags-are-stepic]
└─$ stepic -d -i upz.png
/usr/lib/python3/dist-packages/PIL/Image.py:3368: DecompressionBombWarning: Image size (150658990 pixels) exceeds limit of 89478485 pixels, could be decompression bomb DOS attack.
  warnings.warn(
picoCTF{fl4g_h45_fl4g00518d32} 

```


## Respuesta: **picoCTF{fl4g_h45_fl4g00518d32}**
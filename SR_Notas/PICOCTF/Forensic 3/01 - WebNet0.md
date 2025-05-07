
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

Hints:
Try using a tool like Wireshark.
How can you decrypt the TLS stream?


**Solución 1**

```

Abrir el archivo capture.pcap en wireshark

Menú de arriba, edit, preferences, RSA Key, add new key file, seleccionar la llave que descargamos

Cerrar wireshark, volver a abrirlo con el mismo archivo (capture.pcap), se van a agregar unas nuevas cosas color verde


Seleccionar el no. 32, entrar a Hypertext Transfer Protocol

```



## Respuesta: **picoCTF{nongshim.shrimp.crackers}**





The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the information from this strange file?Download the suspicious file [here](https://artifacts.picoctf.net/c_titan/96/flag2of2-final.pdf).


This problem can be solved by just opening the file in different ways


**Solución 1**

```
┌──(kali㉿kali)-[~/forensic/tarea-forensic/Secret-of-the-Polyglot]
└─$ convert flag2of2-final.pdf flag2of2-final.png 


Abriendo el pdf (archivo original) viene la ultima parte de la bandera, convirtiendo el archivo a png viene la primer parte de la bandera

pdf: 1n_pn9_&_pdf_90974127}
png: picoCTF{f1u3n7_

```



## Respuesta: **picoCTF{f1u3n7_1n_pn9_&_pdf_90974127}**
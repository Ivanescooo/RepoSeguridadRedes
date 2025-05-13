
How about some hide and seek?Download this file [here](https://artifacts.picoctf.net/c_titan/5/unknown.zip).


Hints:
How can you view the information about the picture?
If something isn't in the expected form, maybe it deserves attention?


**Solución 1**

```
┌──(kali㉿kali)-[~/forensic/tarea-forensic/canyousee]
└─$ exiftool ukn_reality.jpg 
ExifTool Version Number         : 13.00
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.3 MB
File Modification Date/Time     : 2024:02:15 17:40:17-05:00
File Access Date/Time           : 2024:02:15 17:40:17-05:00
File Inode Change Date/Time     : 2025:05:12 15:17:05-04:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fNGRhYmRkY2J9Cg==
Image Width                     : 4308
Image Height                    : 2875
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 4308x2875
Megapixels                      : 12.4




Copiar el valor de Attribution URL en cyberchef :
cGljb0NURntNRTc0RDQ3QV9ISUREM05fNGRhYmRkY2J9Cg==

Entrada: cGljb0NURntNRTc0RDQ3QV9ISUREM05fNGRhYmRkY2J9Cg==

From base64:

Salida: picoCTF{ME74D47A_HIDD3N_4dabddcb}

```



## Respuesta: **picoCTF{ME74D47A_HIDD3N_4dabddcb}**
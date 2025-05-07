
We found this [file](https://mercury.picoctf.net/static/09a86202e72dbdb5bf4d1b5d2c6a5b86/tunn3l_v1s10n). Recover the flag.


Weird that it won't display right...


**Solución 1**

```
Abrir hexeditor, con el archivo descargado, las primeras 5 lineas deben estar así:

00000000  42 4D 8E 26  2C 00 00 00   00 00 36 00  00 00 38 00                             BM.&,.....6...8.
00000010  00 00 6E 04  00 00 42 03   00 00 01 00  18 00 00 00                             ..n...B.........
00000020  00 00 58 26  2C 00 25 16   00 00 25 16  00 00 00 00                             ..X&,.%...%.....
00000030  00 00 00 00  00 00 23 1A   17 27 1E 1B  29 20 1D 2A                             ......#..'..) .*
00000040  21 1E 26 1D  1A 31 28 25   35 2C 29 33  2A 27 38 2F                             !.&..1(%5,)3*'8/
00000050  2C 2F 26 23  33 2A 26 2D   24 20 3B 32  2E 32 29 25                             ,/&#3*&-$ ;2.2)%


Después abrir la imagen

```


## Respuesta: **picoCTF{qu1t3_a_v13w_2020}**




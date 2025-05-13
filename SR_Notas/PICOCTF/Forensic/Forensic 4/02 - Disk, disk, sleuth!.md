
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/ac394d24f88e51a09cc909687cf6d853/dds1-alpine.flag.img.gz)

Hints:
Have you ever used `file` to determine what a file was?
Relevant terminal-fu in picoGym: https://play.picoctf.org/practice/challenge/85
Mastering this terminal-fu would enable you to find the flag in a single command: https://play.picoctf.org/practice/challenge/48
Using your own computer, you could use qemu to boot from this disk!


**Solución 1**

```
┌──(kali㉿kali)-[~/forensic/disk-disk-sleuth]
└─$ gzip -d dds1-alpine.flag.img.gz

┌──(kali㉿kali)-[~/forensic/disk-disk-sleuth]
└─$ srch_strings dds1-alpine.flag.img| grep pico
ffffffff81399ccf t pirq_pico_get
ffffffff81399cee t pirq_pico_set
ffffffff820adb46 t pico_router_probe
  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}

```



## Respuesta: **picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}**
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.


Hints:
Remember the flag format is picoCTF{XXXX}

What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)


**Solución 1**

```

ivanesco-picoctf@webshell:~$ nc  jupiter.challenges.picoctf.org 7480 > datos
^C
ivanesco-picoctf@webshell:~$ ls
README.txt  datos  file  flag
ivanesco-picoctf@webshell:~$ cat datos | grep pico
picoCTF{digital_plumb3r_06e9d954}
ivanesco-picoctf@webshell:~$
```


## Respuesta: **picoCTF{digital_plumb3r_06e9d954}**
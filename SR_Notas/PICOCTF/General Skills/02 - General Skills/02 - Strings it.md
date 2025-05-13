
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?

[strings](https://linux.die.net/man/1/strings)


**Solución 1**

```
ivanesco-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
--2025-02-18 20:16:13--  https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 776032 (758K) [application/octet-stream]
Saving to: 'strings'

strings              100%[====================>] 757.84K  1.86MB/s    in 0.4s    

2025-02-18 20:16:13 (1.86 MB/s) - 'strings' saved [776032/776032]

ivanesco-picoctf@webshell:~$ chmod +x strings

ivanesco-picoctf@webshell:~$ strings strings | grep pico

picoCTF{5tRIng5_1T_7f766a23}


```


## Respuesta: **picoCTF{5tRIng5_1T_7f766a23}**

Fix the syntax error in this Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/26/fixme1.py)


Hints:
Indentation is very meaningful in Python

To view the file in the webshell, do: `$ nano fixme1.py`

To exit `nano`, press Ctrl and x and follow the on-screen prompts.

The `str_xor` function does not need to be reverse engineered for this challenge.


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/26/fixme1.py
--2025-02-20 23:14:38--  https://artifacts.picoctf.net/c/26/fixme1.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.42, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 837 [application/octet-stream]
Saving to: 'fixme1.py'

fixme1.py                                            100%[=====================================================================================================================>]     837  --.-KB/s    in 0s      

2025-02-20 23:14:38 (47.8 MB/s) - 'fixme1.py' saved [837/837]


ivanesco-picoctf@webshell:~$ python3 fixme1.py 
  File "/home/ivanesco-picoctf/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent

ivanesco-picoctf@webshell:~$ python3 fixme1.py 
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_09ee727a}

```

Notas: Meterse al archivo y quitar la identación de la línea que imprime la bandera (última línea)

## Respuesta: **picoCTF{1nd3nt1ty_cr1515_09ee727a}**
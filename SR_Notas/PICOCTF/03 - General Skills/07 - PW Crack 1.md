
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.


Hints:
To view the file in the webshell, do: `$ nano level1.py`

To exit `nano`, press Ctrl and x and follow the on-screen prompts.

The `str_xor` function does not need to be reverse engineered for this challenge.


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/11/level1.py
--2025-02-20 23:38:18--  https://artifacts.picoctf.net/c/11/level1.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.93, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 876 [application/octet-stream]
Saving to: 'level1.py'

level1.py                                            100%[=====================================================================================================================>]     876  --.-KB/s    in 0s      

2025-02-20 23:38:18 (833 MB/s) - 'level1.py' saved [876/876]

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
--2025-02-20 23:38:27--  https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.42, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 30 [application/octet-stream]
Saving to: 'level1.flag.txt.enc'

level1.flag.txt.enc                                  100%[=====================================================================================================================>]      30  --.-KB/s    in 0s      

2025-02-20 23:38:27 (32.5 MB/s) - 'level1.flag.txt.enc' saved [30/30]


ivanesco-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: dd
That password is incorrect
ivanesco-picoctf@webshell:~$ nano level1.py
ivanesco-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_fa343060}




```

Notas: la contraseña viene en el archivo python.


## Respuesta: **picoCTF{545h_r1ng1ng_fa343060}**
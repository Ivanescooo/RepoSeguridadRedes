
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.


Hints:
Does that encoding look familiar?

The `str_xor` function does not need to be reverse engineered for this challenge.




**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/13/level2.py
--2025-02-21 00:04:10--  https://artifacts.picoctf.net/c/13/level2.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.93, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 914 [application/octet-stream]
Saving to: 'level2.py'

level2.py                                            100%[=====================================================================================================================>]     914  --.-KB/s    in 0s      

2025-02-21 00:04:10 (640 MB/s) - 'level2.py' saved [914/914]

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/13/level2.flag.txt.enc
--2025-02-21 00:04:27--  https://artifacts.picoctf.net/c/13/level2.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.71, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 31 [application/octet-stream]
Saving to: 'level2.flag.txt.enc'

level2.flag.txt.enc                                  100%[=====================================================================================================================>]      31  --.-KB/s    in 0s      

2025-02-21 00:04:27 (12.3 MB/s) - 'level2.flag.txt.enc' saved [31/31]

ivanesco-picoctf@webshell:~$ nano level2.py
ivanesco-picoctf@webshell:~$ python3 level2.py 
Please enter correct password for flag: de76
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}


```

Notas: pasar la contraseña con formato chr(0xNN) 

## Respuesta: **picoCTF{tr45h_51ng1ng_489dea9a}**


Referencias: https://gchq.github.io/CyberChef/
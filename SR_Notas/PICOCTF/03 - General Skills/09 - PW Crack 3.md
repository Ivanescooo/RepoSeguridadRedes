
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/16/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/16/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/16/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.



Hints:
To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`

To exit `bvi` type `:q` and press enter.

The `str_xor` function does not need to be reverse engineered for this challenge.



**Solución 1**

```
ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/16/level3.py
--2025-02-21 03:16:56--  https://artifacts.picoctf.net/c/16/level3.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.93, 3.160.5.71, 3.160.5.42, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.93|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1337 (1.3K) [application/octet-stream]
Saving to: 'level3.py'

level3.py                                            100%[=====================================================================================================================>]   1.31K  --.-KB/s    in 0s      

2025-02-21 03:16:56 (89.6 MB/s) - 'level3.py' saved [1337/1337]

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/16/level3.flag.txt.enc
--2025-02-21 03:17:07--  https://artifacts.picoctf.net/c/16/level3.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.93, 3.160.5.71, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 31 [application/octet-stream]
Saving to: 'level3.flag.txt.enc'

level3.flag.txt.enc                                  100%[=====================================================================================================================>]      31  --.-KB/s    in 0s      

2025-02-21 03:17:07 (2.13 MB/s) - 'level3.flag.txt.enc' saved [31/31]

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/16/level3.hash.bin
--2025-02-21 03:17:15--  https://artifacts.picoctf.net/c/16/level3.hash.bin
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.93, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 16 [application/octet-stream]
Saving to: 'level3.hash.bin'

level3.hash.bin                                      100%[=====================================================================================================================>]      16  --.-KB/s    in 0s      

2025-02-21 03:17:15 (1004 KB/s) - 'level3.hash.bin' saved [16/16]


ivanesco-picoctf@webshell:~$ nano level3.py
ivanesco-picoctf@webshell:~$ python3 level3.py 
That password is incorrect
That password is incorrect
That password is incorrect
That password is incorrect
That password is incorrect
That password is incorrect
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_2b072a90}

```



## Respuesta: **picoCTF{m45h_fl1ng1ng_2b072a90}**
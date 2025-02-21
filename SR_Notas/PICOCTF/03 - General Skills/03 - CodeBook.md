
Run the Python script `code.py` in the same directory as `codebook.txt`.

- [Download code.py](https://artifacts.picoctf.net/c/2/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/2/codebook.txt)


Hints:
On the webshell, use `ls` to see if both files are in the directory you are in
The `str_xor` function does not need to be reverse engineered for this challenge.



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/2/code.py
--2025-02-20 23:03:52--  https://artifacts.picoctf.net/c/2/code.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.42, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1278 (1.2K) [application/octet-stream]
Saving to: 'code.py'

code.py                                              100%[=====================================================================================================================>]   1.25K  --.-KB/s    in 0s      

2025-02-20 23:03:52 (23.8 MB/s) - 'code.py' saved [1278/1278]

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/2/codebook.txt
--2025-02-20 23:04:01--  https://artifacts.picoctf.net/c/2/codebook.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.18, 3.160.5.42, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 27 [application/octet-stream]
Saving to: 'codebook.txt'

codebook.txt                                         100%[=====================================================================================================================>]      27  --.-KB/s    in 0s      

2025-02-20 23:04:01 (1.27 MB/s) - 'codebook.txt' saved [27/27]

ivanesco-picoctf@webshell:~$ python3 code.py    
picoCTF{c0d3b00k_455157_7d102d7a}

```



## Respuesta: **picoCTF{c0d3b00k_455157_7d102d7a}**

Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/504/big-zip-files.zip)

Can grep be instructed to look at every file in a directory and its subdirectories?


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/504/big-zip-files.zip
--2025-02-19 02:19:35--  https://artifacts.picoctf.net/c/504/big-zip-files.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.43, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3182988 (3.0M) [application/octet-stream]
Saving to: 'big-zip-files.zip'

big-zip-files.zip                                    100%[=====================================================================================================================>]   3.04M  1.82MB/s    in 1.7s    

2025-02-19 02:19:36 (1.82 MB/s) - 'big-zip-files.zip' saved [3182988/3182988]

ivanesco-picoctf@webshell:~$ unzip big-zip-files.zip 


ivanesco-picoctf@webshell:~$ grep -R picoCTF{
big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}

```


## Respuesta: **picoCTF{gr3p_15_m4g1c_ef8790dc}**
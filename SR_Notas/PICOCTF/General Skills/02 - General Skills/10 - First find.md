

Unzip this archive and find the file named 'uber-secret.txt'

- [Download zip file](https://artifacts.picoctf.net/c/502/files.zip)

(None)


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/502/files.zip
--2025-02-19 02:21:19--  https://artifacts.picoctf.net/c/502/files.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.43, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3995553 (3.8M) [application/octet-stream]
Saving to: 'files.zip'

files.zip                                            100%[=====================================================================================================================>]   3.81M  1.82MB/s    in 2.1s    

2025-02-19 02:21:22 (1.82 MB/s) - 'files.zip' saved [3995553/3995553]

ivanesco-picoctf@webshell:~$ unzip files.zip 

ivanesco-picoctf@webshell:~/files$ cat files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}



```




**Solución 2**


```

ivanesco-picoctf@webshell:~/files$ find . -name uber-secret.txt
./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
ivanesco-picoctf@webshell:~/files$ cat ./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}

```

## Respuesta: **picoCTF{f1nd_15_f457_ab443fd1}**
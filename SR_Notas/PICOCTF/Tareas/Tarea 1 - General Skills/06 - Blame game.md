
Someone's commits seems to be preventing the program from working. Who is it?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/159/challenge.zip)


Hints:
In collaborative projects, many users can make many changes. How can you see the changes within one file?

Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).

You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/159/challenge.zip
--2025-02-22 05:32:38--  https://artifacts.picoctf.net/c_titan/159/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.93, 3.160.5.71, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.93|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 293915 (287K) [application/octet-stream]
Saving to: 'challenge.zip'

challenge.zip                                        100%[=====================================================================================================================>] 287.03K  --.-KB/s    in 0.1s    

2025-02-22 05:32:38 (1.92 MB/s) - 'challenge.zip' saved [293915/293915]

ivanesco-picoctf@webshell:~$ unzip challenge.zip 


ivanesco-picoctf@webshell:~$ cd drop-in/
ivanesco-picoctf@webshell:~/drop-in$ git log message.py

picoCTF{@sk_th3_1nt3rn_81e716ff}

```



## Respuesta: **picoCTF{@sk_th3_1nt3rn_81e716ff}**
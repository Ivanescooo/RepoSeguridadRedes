
What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/161/challenge.zip)


Hints:
The `cat` command will let you read a file, but that won't help you here!

Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).

When committing a file with git, a message can (and should) be included.


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/161/challenge.zip
--2025-02-22 05:29:06--  https://artifacts.picoctf.net/c_titan/161/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.18, 3.160.5.42, 3.160.5.93, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 17739 (17K) [application/octet-stream]
Saving to: 'challenge.zip'

challenge.zip                                        100%[=====================================================================================================================>]  17.32K  --.-KB/s    in 0.007s  

2025-02-22 05:29:06 (2.56 MB/s) - 'challenge.zip' saved [17739/17739]

ivanesco-picoctf@webshell:~$ unzip challenge.zip 

ivanesco-picoctf@webshell:~$ cd drop-in/
ivanesco-picoctf@webshell:~/drop-in$ git log


```



## Respuesta: **picoCTF{t1m3m@ch1n3_8defe16a}**
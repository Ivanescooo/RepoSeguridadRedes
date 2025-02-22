
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/69/challenge.zip)


Hints:
`git branch -a` will let you see available branches

How can file 'diffs' be brought to the main branch? Don't forget to `git config`!

Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/69/challenge.zip
--2025-02-22 05:39:20--  https://artifacts.picoctf.net/c_titan/69/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.18, 3.160.5.93, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 24642 (24K) [application/octet-stream]
Saving to: 'challenge.zip'

challenge.zip                                        100%[=====================================================================================================================>]  24.06K  --.-KB/s    in 0.01s   

2025-02-22 05:39:20 (2.32 MB/s) - 'challenge.zip' saved [24642/24642]

ivanesco-picoctf@webshell:~$ unzip challenge.zip 


ivanesco-picoctf@webshell:~$ cd drop-in/
ivanesco-picoctf@webshell:~/drop-in$ git branch -a


ivanesco-picoctf@webshell:~/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
ivanesco-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')ivanesco-picoctf@webshell:~/drop-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'
ivanesco-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")

print("m@k3s_th3_dr3@m_", end='')ivanesco-picoctf@webshell:~/drop-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'
ivanesco-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")

print("w0rk_e4b79efb}")



picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_e4b79efb}



```




## Respuesta: **picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_e4b79efb}**
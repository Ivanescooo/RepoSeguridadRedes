
Fix the syntax error in the Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/5/fixme2.py)


Hints:
Are equality and assignment the same symbol?

To view the file in the webshell, do: `$ nano fixme2.py`

To exit `nano`, press Ctrl and x and follow the on-screen prompts.

The `str_xor` function does not need to be reverse engineered for this challenge.



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/5/fixme2.py
--2025-02-20 23:31:38--  https://artifacts.picoctf.net/c/5/fixme2.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.71, 3.160.5.18, 3.160.5.42, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.71|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1029 (1.0K) [application/octet-stream]
Saving to: 'fixme2.py'

fixme2.py                                            100%[=====================================================================================================================>]   1.00K  --.-KB/s    in 0s      

2025-02-20 23:31:38 (41.3 MB/s) - 'fixme2.py' saved [1029/1029]

ivanesco-picoctf@webshell:~$ python3 fixme2.py 
  File "/home/ivanesco-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?


ivanesco-picoctf@webshell:~$ nano fixme2.py 
ivanesco-picoctf@webshell:~$ python3 fixme2.py 
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
ivanesco-picoctf@webshell:~$ 


```

Notas: modificar el IF indicado, ya que solo tiene un símbolo de igual y deben de ser 2 

## Respuesta: **picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}**
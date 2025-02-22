
I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/136/challenge.zip)


Hints:
Version control can help you recover files if you change or lose them!

Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)

You can 'checkout' commits to see the files inside them



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/136/challenge.zip
--2025-02-22 04:34:14--  https://artifacts.picoctf.net/c_titan/136/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.42, 3.160.5.93, 3.160.5.18, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.42|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 19196 (19K) [application/octet-stream]
Saving to: 'challenge.zip'

challenge.zip                                        100%[=====================================================================================================================>]  18.75K  --.-KB/s    in 0.007s  

2025-02-22 04:34:14 (2.78 MB/s) - 'challenge.zip' saved [19196/19196]

ivanesco-picoctf@webshell:~$ unzip challenge.zip 

ivanesco-picoctf@webshell:~$ cd drop-in/


ivanesco-picoctf@webshell:~/drop-in$ git reflog
ivanesco-picoctf@webshell:~/drop-in$ git checkout 87b85d7
Note: switching to '87b85d7'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 87b85d7 create flag

ivanesco-picoctf@webshell:~/drop-in$ cat message.txt 
picoCTF{s@n1t1z3_ea83ff2a}


```


## Respuesta: **picoCTF{s@n1t1z3_ea83ff2a}**



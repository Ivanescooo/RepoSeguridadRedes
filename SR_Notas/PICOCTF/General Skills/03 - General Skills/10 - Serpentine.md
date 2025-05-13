

Find the flag in the Python script!


Hints: 
Try running the script and see what happens

In the webshell, try examining the script with a text editor like `nano`

To exit `nano`, press Ctrl and x and follow the on-screen prompts.

The `str_xor` function does not need to be reverse engineered for this challenge.


**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/37/serpentine.py
--2025-02-21 03:40:39--  https://artifacts.picoctf.net/c/37/serpentine.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.93, 3.160.5.18, 3.160.5.71, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.93|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 2550 (2.5K) [application/octet-stream]
Saving to: 'serpentine.py'

serpentine.py                                        100%[=====================================================================================================================>]   2.49K  --.-KB/s    in 0s      

2025-02-21 03:40:40 (1.64 GB/s) - 'serpentine.py' saved [2550/2550]

ivanesco-picoctf@webshell:~$ python3 serpentine.py 

    Y
  .-^-.
 /     \      .- ~ ~ -.
()     ()    /   _ _   `.                     _ _ _
 \_   _/    /  /     \   \                . ~  _ _  ~ .
   | |     /  /       \   \             .' .~       ~-. `.
   | |    /  /         )   )           /  /             `.`.
   \ \_ _/  /         /   /           /  /                `'
    \_ _ _.'         /   /           (  (
                    /   /             \  \
                   /   /               \  \
                  /   /                 )  )
                 (   (                 /  /
                  `.  `.             .'  /
                    `.   ~ - - - - ~   .'
                       ~ . _ _ _ _ . ~

Welcome to the serpentine encourager!


a) Print encouragement
b) Print flag
c) Quit

What would you like to do? (a/b/c) c


ivanesco-picoctf@webshell:~$ nano serpentine.py 

ivanesco-picoctf@webshell:~$ python3 serpentine.py 

    Y
  .-^-.
 /     \      .- ~ ~ -.
()     ()    /   _ _   `.                     _ _ _
 \_   _/    /  /     \   \                . ~  _ _  ~ .
   | |     /  /       \   \             .' .~       ~-. `.
   | |    /  /         )   )           /  /             `.`.
   \ \_ _/  /         /   /           /  /                `'
    \_ _ _.'         /   /           (  (
                    /   /             \  \
                   /   /               \  \
                  /   /                 )  )
                 (   (                 /  /
                  `.  `.             .'  /
                    `.   ~ - - - - ~   .'
                       ~ . _ _ _ _ . ~

Welcome to the serpentine encourager!


a) Print encouragement
b) Print flag
c) Quit

What would you like to do? (a/b/c) b
picoCTF{7h3_r04d_l355_7r4v3l3d_8e47d128}
a) Print encouragement
b) Print flag
c) Quit


```



## Respuesta: **picoCTF{7h3_r04d_l355_7r4v3l3d_8e47d128}**
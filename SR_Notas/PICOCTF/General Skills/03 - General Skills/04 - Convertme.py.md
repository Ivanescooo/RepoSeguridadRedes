
Run the Python script and convert the given number from decimal to binary to get the flag.[Download Python script](https://artifacts.picoctf.net/c/23/convertme.py)


Hints:
Look up a decimal to binary number conversion app on the web or use your computer's calculator!

The `str_xor` function does not need to be reverse engineered for this challenge.

If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.

To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'

Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!

Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 convertme.py`



**Solución 1**

```

ivanesco-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/23/convertme.py
--2025-02-20 23:10:24--  https://artifacts.picoctf.net/c/23/convertme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.5.18, 3.160.5.93, 3.160.5.71, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.5.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1189 (1.2K) [application/octet-stream]
Saving to: 'convertme.py'

convertme.py                                         100%[=====================================================================================================================>]   1.16K  --.-KB/s    in 0s      

2025-02-20 23:10:24 (88.1 MB/s) - 'convertme.py' saved [1189/1189]

ivanesco-picoctf@webshell:~$ python3 convertme.py 
If 91 is in decimal base, what is it in binary base?
Answer: 01011011
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_9c3b7d4d}

```


## Respuesta: **picoCTF{4ll_y0ur_b4535_9c3b7d4d}**


Referencias: https://gchq.github.io/CyberChef/
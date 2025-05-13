
I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_atlas/2/challenge.zip)

The same files are accessible via SSH here:`ssh -p 55872 ctf-player@atlas.picoctf.net`Using the password `1ad5be0d`. Accept the fingerprint with `yes`, and `ls` once connected to begin. Remember, in a shell, passwords are hidden!



Hints:
QR codes are a way of encoding data. While they're most known for storing URLs, they can store other things too.
Mobile phones have included native QR code scanners in their cameras since version 8 (Oreo) and iOS 11
If you don't have access to a phone, you can also use zbar-tools to convert an image to text


**Solución 1**

```
──(kali㉿kali)-[~/…/scan-me/home/ctf-player/drop-in]
└─$ ssh -p 55872 ctf-player@atlas.picoctf.net
The authenticity of host '[atlas.picoctf.net]:55872 ([18.217.83.136]:55872)' can't be established.
ED25519 key fingerprint is SHA256:hVmbk/OaNT4902bBr7h26wfhmBuJWi4tub8AJqoAJCM.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? y
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added '[atlas.picoctf.net]:55872' (ED25519) to the list of known hosts.
ctf-player@atlas.picoctf.net's password: 


Aquí sale el codigo QR


ctf-player@challenge:~/drop-in$ zbarimg flag.png 
Connection Error (Failed to connect to socket /var/run/dbus/system_bus_socket: No such file or directory)
Connection Null
QR-Code:picoCTF{p33k_@_b00_b5ce2572}
scanned 1 barcode symbols from 1 images in 0 seconds



```



## Respuesta: **picoCTF{p33k_@_b00_b5ce2572}**
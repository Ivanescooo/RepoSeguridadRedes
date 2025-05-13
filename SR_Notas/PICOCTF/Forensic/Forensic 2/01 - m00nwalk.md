
Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.


Hints:
How did pictures from the moon landing get sent back to Earth?

What is the CMU mascot?, that might help select a RX option



**Solución 1**

```

──(kali㉿kali)-[~/forensic/forensic2/moonwalk]
└─$ cd /opt  

(kali㉿kali)-[/opt]
└─$ sudo  git clone https://github.com/colaclanth/sstv.git

(kali㉿kali)-[/opt]
└─$ cd sstv 
                                                                                                          
┌──(kali㉿kali)-[/opt/sstv]
└─$ sudo python3 setup.py install

──(kali㉿kali)-[~/forensic/forensic2/moonwalk]
└─$ sstv -d message.wav -o result.png
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [########################################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!

(kali㉿kali)-[~/forensic/forensic2/moonwalk]
└─$ open result.png



Se abre la imagen y tenemos que voltearla, así se va clara la bandera.

```



## Respuesta: **picoCTF{beep_boop_im_in_space}**




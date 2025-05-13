

Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:21485/](http://mercury.picoctf.net:21485/)


None



**Solución 1**

```

 for i in {1..30}; do echo $i ; curl -s http://mercury.picoctf.net:21485/check -H "Cookie: name=$i"; done | grep 'picoCTF{'
 
<p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}</code></p>


```


## Respuesta: **picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}**

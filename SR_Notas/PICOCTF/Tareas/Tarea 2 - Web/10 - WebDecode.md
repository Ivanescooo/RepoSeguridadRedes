
Do you know how to use the web inspector?Start searching [here](http://titan.picoctf.net:59355/) to find the flag


Hints:
Use the web inspector on other files included by the web page.

The flag may or may not be encoded



**Solución 1**

```

Hay 3 botones arriba a la derecha, dar click al "about"

ver código fuente, está esta linea de código: 
|   |
|---|
|<section class="about" notify_true="cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfZGYwZGE3Mjd9">|
||<h1>|

transformar el texto entre comillas

Input: cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfZGYwZGE3Mjd9

Recipe: 
	From Base 64

picoCTF{web_succ3ssfully_d3c0ded_df0da727}


```


## Respuesta: **picoCTF{web_succ3ssfully_d3c0ded_df0da727}**



To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with `nc jupiter.challenges.picoctf.org 15130`.


Hints:
I hear python can convert things.
It might help to have multiple windows open.


**Solución 1**

```
ivanesco-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 15130
Let us see how data is stored
pie
Please give the 01110000 01101001 01100101 as a word.
...
you have 45 seconds.....

Input:
pie
Please give me the  143 157 155 160 165 164 145 162 as a word.
Input:
computer
Please give me the 6c69676874 as a word.
Input:
light
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_02167de8}


```

Notas: para obtener las palabras en base a los valores se usó cyberchef 

## Respuesta: **picoCTF{learning_about_converting_values_02167de8}**


Referencias

https://gchq.github.io/CyberChef/
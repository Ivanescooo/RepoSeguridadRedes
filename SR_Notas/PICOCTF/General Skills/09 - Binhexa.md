
How well can you perfom basic binary operations?Start searching for the flag here `nc titan.picoctf.net 64198`


(None)


**Solución 1**

```

ivanesco-picoctf@webshell:~$ nc titan.picoctf.net 64198

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10110101
Binary Number 2: 11100100


Question 1/6:
Operation 1: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 01010000100110100
Correct!

Question 2/6:
Operation 2: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 101101010
Correct!

Question 3/6:
Operation 3: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10100100
Correct!

Question 4/6:
Operation 4: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11110101
Correct!

Question 5/6:
Operation 5: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 110011001
Correct!

Question 6/6:
Operation 6: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 1110010
Correct!

Enter the results of the last operation in hexadecimal: 72

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d9a7ddd2}

```



## Respuesta: **picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d9a7ddd2}**



Referencias:
https://www.rapidtables.com/calc/math/binary-calculator.html


Now you DON’T see me.This [report](https://artifacts.picoctf.net/c/84/Financial_Report_for_ABC_Labs.pdf) has some critical data in it, some of which have been redacted correctly, while some were not. Can you find an important key that was not redacted properly?


How can you be sure of the redaction?


**Solución 1**

```
┌──(kali㉿kali)-[~/forensic/tarea-forensic/redaction-gone-wrong]
└─$ sudo apt install poppler-utils

                                                                                                         
┌──(kali㉿kali)-[~/forensic/tarea-forensic/redaction-gone-wrong]
└─$ pdftotext Financial_Report_for_ABC_Labs.pdf 
                                                                                                          
┌──(kali㉿kali)-[~/forensic/tarea-forensic/redaction-gone-wrong]
└─$ ls
Financial_Report_for_ABC_Labs.pdf  Financial_Report_for_ABC_Labs.txt
                                                                                                          
┌──(kali㉿kali)-[~/forensic/tarea-forensic/redaction-gone-wrong]
└─$ cat Financial_Report_for_ABC_Labs.txt
Financial Report for ABC Labs, Kigali, Rwanda for the year 2021.
Breakdown - Just painted over in MS word.

Cost Benefit Analysis
Credit Debit
This is not the flag, keep looking
Expenses from the
picoCTF{C4n_Y0u_S33_m3_fully}
Redacted document.


```



## Respuesta: **picoCTF{C4n_Y0u_S33_m3_fully}**
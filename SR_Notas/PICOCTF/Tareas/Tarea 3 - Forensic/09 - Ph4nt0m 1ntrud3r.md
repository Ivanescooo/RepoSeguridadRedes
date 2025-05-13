
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/bdda31c79c31975a5fe5402777bc87794655172e5d5bb2b569f1970df8efda34/myNetworkTraffic.pcap) and try to get the flag.


Hints:
Filter your packets to narrow down your search.
Attacks were done in timely manner.
Time is essential


**Solución 1**

```
Usando tshark:

┌──(kali㉿kali)-[~/forensic/tarea-forensic/ph4nt0m]
└─$ tshark -r myNetworkTraffic.pcap -Y "tcp.len==12 || tcp.len==4" -T fields -e frame.time -e tcp.segment_data | sort -k4 | awk '{print $6}' | xxd -p -r | base64 -d
Warning: program compiled against libxml 212 using older 209
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_af160980} 

```



## Respuesta: **picoCTF{1t_w4snt_th4t_34sy_tbh_4r_af160980} **
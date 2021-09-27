# Inside-Out

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-33-52.png)

# Vulnerability
So, first of all, i was just playing around to find interesting about challenge. And i found two interesting.

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-20-20.png)

the first one is (/admin) part. when I go to it, it was Forbidden by saying that "Only accessible from the local network". 

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-20-43.png)


The second thing that i found is (proxy-service).  This proxy will show all the info and response about website that we want to get. Cool!

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-21-08.jpg)

We can see there is a 'request' parameter that we can change the url which we want to go. 

So, i am sured that this is SSRF vulnerability. Let pwn this!

# Solution

So i tested by (http://localhost/admin). but it was blacklist. 

So i find the resources to bypass it, and i found blog post form HackTricks. (https://book.hacktricks.xyz/pentesting-web/ssrf-server-side-request-forgery)

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-21-24.png)

So i found (http://0.0.0.0/admin) to bypass this blacklist. So i used it and got flag.

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Inside-Out/Screenshot%20from%202021-09-26%2022-21-42.jpg)

# flag
DUCTF{very_spooky_request}

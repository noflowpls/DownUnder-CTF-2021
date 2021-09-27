# Cowboy World

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-41-34.png)

# Vulnerability
Honestly, i didn't really know what type of vulnerability until now even i solved it. 😂

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-41-45.png)

# Solution

I am just playing around the website And i found (/robots.txt) that leads to another web path called (/sad.eml)

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-42-01.png)

When I go to it, i got (.eml) email file 

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-44-51.jpg)

I looked into the email file.
![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-46-00.png)

I knew the email is send to sadcowboys@gmail.com. And i noticed the letters in the line of 18,

said that "thats why a 'sadcowboy' is only allowed to go into our website". 

So i knew that username is sadcowboy.

But i can't find the password, so i just testing some default passwords and  i got one idea that why i don't try sql injection in password field.

So I used (sadcowboy) for username and for password i used (' or 1=1 --).

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-46-29.png)

Well, you can tell that i am lucky because in my first try with sql injection, It worked! Perfect!

![ctf](https://github.com/ComdeyOverFlow/DownUnder-CTF-2021/blob/main/Cowboy-World/images/Screenshot%20from%202021-09-27%2002-46-36.png)

I really like this challenge. Thanks to all of CTF-organizers.

# Thanks For reading!

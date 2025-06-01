# Red Team


## Disclaimer

This game is for educational purposes only. Unauthorized use of the tools that are incorporated into the game is illegal. The story is fictitious.

### Introduction Level
Welcome! This training will teach you how attackers use reconnaissance, weak configurations, and privilege escalation to compromise systems!
Story: You and your friends are fans of a series that aired last week. Recently, your friend Ivan ruined the fun by spoiling the finale before you could watch it! He runs a server where he stores his collection of movies and series, and you've decided to get some friendly revenge by limiting his access to the server. Let's teach Ivan a lesson about cybersecurity while having a little fun. :)

### Get Access
Firstly, let's access the Kali Linux machine we will use for the training!
A window with a topology should appear on your right, showing available machines and networks.

You will have access only to the attacker machine (if you don’t see the machine immediately, click on the switches, and it should appear).
To access the attacker machine, right-click it and select console (deprecated)—this will open a tab with the Kali Linux starting machine.
Your login credentials for the attacker machine are:
Username: Sandy
Password: sandypass
After logging into the attacker machine, open the terminal.

### Initial Reconnaissance
You overheard Ivan bragging about how secure his server is. However, you overheard him casually mention his server's IP address: 10.1.26.9. Using basic tools, you run a network scan to uncover the services he left open.

**Objective:** To progress further, use a tool for port scanning and execute a command that shows the running services and some information about them on Ivan’s server. Type in the entire command in the answer box!

### Gaining Access
By running nmap, we discovered an open FTP port (21) on the server. Interesting. File Transfer Protocol (FTP) is a standard communication protocol used for transferring files from a server to a client on a computer network.
Since Ivan isn’t the kind of guy who reads about protocols' vulnerabilities, let's see whether he has left his FTP server open to anonymous logins.

**Objective:** Try logging into Ivan's FTP server and look for some files he may have stored. The flag we are looking for is the name of the most interesting-looking file in the FTP server. ;)


### SSH Login
We found an interesting file on Ivan’s server—backup.txt! But to open it and see what’s inside, we must transfer the file to our machine.
After transferring the file, we noticed backup.txt contains user credentials for Ivan’s server! ;)

**Objective:** Let’s try logging in as this user on Ivan’s server. Type in the entire command to log into Ivan’s server.

### Restricting Access
You're in! It looks like the user Ivan has root privileges. ;) it's time to remove his ability to log into the server entirely. He'll be locked out until he fixes his configurations.

**Objective:** Change Ivan’s password to complete your revenge! Type in the entire command to change Ivan’s password (with privileges).

### Good Job!
Ivan is now locked out of his server, and your revenge is complete! :) Of course, he’ll need to call you for help, and that’s when you’ll reveal the prank and teach him the importance of securing his system! :D
I hope this challenge has taught you how attackers use reconnaissance, weak configurations, and privilege escalation to compromise systems. While you've used these skills for a playful prank, remember that such vulnerabilities can lead to serious consequences in the real world. Always secure your systems and respect ethical guidelines! :)


Estimated Duration: 19 minutes

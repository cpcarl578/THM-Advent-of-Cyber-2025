# Advent of Cyber Day 11-XSS-Merry XSSMas

## Objectives

* Understand how XSS works
* Learn How to prevent XSS attacks

### Skills Learned/Lessons learned

* Very basic overview of Reflected XSS (Cross site scripting) and Stored XSS

### Tools used

* Platform used- TryHackMe

## Flags

* THM{Evil_Bunny}
* THM{Evil_Stored_Egg}

### Practical portion

1. Start the attacker machine
2. Start the target machine
3. Open Firefox and navigate to the IP address
4. Read about Reflected XSS
5. Exploit Reflected XSS by using "script alert 'Reflected Meow Meow' /script
6. The page refreshes and displays flag THM{Evil_Bunny}
7. We move on to see if we can use a stored XSS payload and enter into send a message box "script alert ('Stored Meow Meow')/script"
8. The page refreshes and the dialog box is displayed and we are presented with the flag below where we submitted our message  the flag we see is flag THM{Evil_Stored_Egg}

## Takeaways from todays room

I learned about stored and reflected cross site scripting. One of the major dangers is that the website will execute code instead of reading it as text. This web app vulnerability can be used to steal credentials, impersonate users, and deface pages. Stored XSS happens when there is malicious code stored on the server as opposed to reflected which happens immediately. This was a great intro into Cross site scripting and how it works.

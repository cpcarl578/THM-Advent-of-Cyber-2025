#  Day 9-Passwords-A Cracking Christmas

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

1. How password-based encryption protects files like PDF's and ZIP archives
2. Why weak passwords make encrypted files vulnerable 
3. How attackers use dictionary and brute force attacks to recover passwords
4. Hands on cracking the password of an encrypted file to reveal the contents
5. The importance of using strong, complex passwords to defend against these types of attacks.





### Skills Learned/Lessons learned

- Injection Prompting 
- Security risks in using AI

### Tools Used

- Platform used to learn- TryHackMe
- John

## Flags

- "THM{Cr4ck1n6_z1p$_1s_34$yyyy"
- THM{Cr4ck1ng_PDFS_1s_34$y}"
 
### Practical Portion

1. Start the attacker machine took longer today than previous days
2. Start the target machine
3. Read the about how attackers recover weak passwords
4. use command cd desktop
5. run file flag.pdf we are given the number of pages and the version this is using 
6. run file flag.zip we are given the number of pages and the version this is using
7. run "pdfcrack -f flag.pdf -w /usr/share/wordlists/rockyou.txt"
8. we have found the password for this user which is *********** 11 characters all lowercase with no spaces
9. run the command zip2john flag.zip > xiphas.txt
10. run john --wordlist=/usr/share/wordlists/rockyou.txt ziphash.txt
11. output password is *********** 11 characters all lowercase no spaces with one number
12. go to desktop and open the PDF we are asked to enter the password which we obtained up above enter  *********** we are presented with the flag "THM{Cr4ck1ng_PDFS_1s_34$y}"
13. go to desktop and decrypt zip file and enter *********** open file and we are presented with flag "THM{Cr4ck1n6_z1p$_1s_34$yyyy" 



## Takeaways

Todays room was all about learning how to recover weak passwords using dicrionary attacks as well as mask attacks, I enjoyed learning how to do both with the hands on portion. I was able to use this lab today to capture both of the flags using Linux CLI and John the Ripper. I am going to continue with the room suggested (Password Attacks) after I have completed the Advent of Cyber!

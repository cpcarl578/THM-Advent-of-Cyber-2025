# Advent of Cyber Day 17-CyberChef-Hoperation Save McSkidy

## Objectives

* Intro to Decoding and encoding
* Learn how to use cyberchef
* Identify useful information in web applications through HTTP headers 

### Skills Learned/Lessons learned

* Cyberchef receipes
* Crackstation
* Intro to cryptography

### Tools used

* Platform-TryHackMe
* CyberChef
* Crackstation

## Flags

* THM{M3D13V4L_D3C0D3R_4D3P7}

### Practical portion

1. Start attacker machine
2. Start target machine
3. Open cyberchef on attacker machine
4. Drag "To Base64" in the cyberchef receipes
5. Type "Iamroot" into the input section of CyberChef
6. Enable web devolper tools
7. Look at the chat on the left side and we see that the message is in base 64
8. Go to CyberChef and tranfer the plaintext username to base 64 for the username
9. Look at the devolper tools for level one and take the value for what the password is and put that into cyberchef to transfer to base64 and enter that into the chat the chatbot responds in base 64 transfer that to plain text for the username and enter that as the password. we have completed stage 1 
10. Repeat steps for stage 1 
11. Stage 3 there is no magic question displayed in the web dev tools so we need to come up with a question to ask to be given the password.
12. Takes multiple attempts but we are finally given the password in base64
13. Go over to cyberchef and input the value for the password we were given.
14. Use base64 and XOR to gain the correct password.
15. Stage 4 we have the same basic steps to gain the username in base64 but when it comes time to get the password it is in Md5 hash
16. We get the response from the chatbot and go to crackstation and paste the md5 hash
17. Retrieve the password and try that for login didnt work the first time so assuming I made an error
18. Retry the password through crackstation and received the correct password this time
19. Stage 5
20. Obtain the username the same way we have been
21. Ask the chatbot for the password receive it but we have to run that from base64 to from Hex to reverse
22. Had issues receiving the correct password

## Takeaways from todays room

The begining of this room was a little over my head but after the first two examples I got the hang of using Cyberchef to decode from Base64 and plaintext to Base64. This was a good intro into encoding and decoding. After the AOC is complete I will be coming back to the room intro to cryptography. 

# Advent of Cyber Day 21-Malware Analysis-Malhare.exe

## Objectives

Reverse engineer an HTA file and look for-

* Application Metadata
* Script Functions
* Any network calls or encoded data
* Clues about exfil

### Skills Learned/Lessons learned

* Script analysis
* Malware Analysys
* Learned a new command today in Linux

### Tools used

* Platform-TryHackMe
* CyberChef

## Flags

* THM{Malware.Analysed}

### Practical portion

1. Launch the attacker machine
2. Download the HTA malware file in the VM ONLY
3. Went to Terminal and ran command "pluma /root/Rooms/AoC2025/Day21/survey.hta"
4. Take the base64 and input into CyberChef to see what that says we are presented with a link
5. Review the example in pluma on the VM as this file has some data redacted due to safety concerns with the script
6. Answer questions for todays room using the script in question

## Takeaways from todays room

Today was pretty overwhelming to understand for me. I followed the walkthrough and that helped me to grasp some of the concepts discussed in todays room. I really enjoy using CyberChef to try and decode. I am going to continue learning this as its something I am not fully grasping yet and would like to understand more.

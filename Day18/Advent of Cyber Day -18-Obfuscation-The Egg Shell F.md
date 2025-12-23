# Advent of Cyber Day 18-The Egg Shell File

## Objectives

* Learn about obfuscation and why and where it is used
* Learn the difference between encoding,encryption and obfuscation
* Learn about obfuscation and the common techniques
* Use CyberChef to recover plaintext safely

### Skills Learned/Lessons learned

* Further Cyberchef skills
* Magic formula in Cyberchef to help

### Tools used

* TryHackMe
* CyberChef

## Flags

* THM{C2_De0bfuscation_29838}
* THM{API_Obfusc4tion_ftw_0283}

### Practical portion

1. Start the attacker machine
2. Use CyberChef to do a test run using carrot supremacy
3. Make sure the receipe is "XOR" set the key to "a" and make sure hex is selected from drop down menu
4. We receive ikxxe~*y zxogkis as the output
5. Open the file in visual studio and read the instructions
6. Deobfuscate the first line using CyberChef and we receive a link
7. Enter that link into the correct line in visual studio and save
8. Open powershell and run command cd .\Desktop\
9. We are in the desktop directory now as displayed on screen
10. Run command .\SantaStealer.ps1
11. Returns the Flag THM{C2_De0bfuscation_29838}
12. Moving on to the second task which is to obfuscate an apikey and use XOR single byte 0x37 and convert that to hexidecimal
13. Using CyberChef we paste the api key add XOR to our recipe
14. Than add hex to the receipe
15. We have a result for a hexidecimal and add that to the script and save in Visual studio
16. Head back to Windows Powershell and run the script again
17. Receive flag THM{API_Obfusc4tion_ftw_0283}
18. Complete todays room

## Takeaways from todays room

I really enjoyed this room today as it had some followup on some of the concepts that were in yesterdays room. I enjoy using CyberChef and think this is going to be a very useful tool for me. I am going to continue learning hashes and obfuscation as these two topics are topics that I did not know much about before the Advent of Cyber 2025 and want to continue learning these techniques.

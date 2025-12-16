# Advent of Cyber Day 13-YARA Rules-YARA mean one!

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

* Understand the basic concept of YARA.
* Learn when and why we need to use YARA rules.
* Explore different types of YARA rules.
* Learn how to write YARA rules.
* Practically detect malicious indicators using YARA.

### Skills Learned/Lessons learned

* Exposure to YARA rules and how they work
* Basic editing of YARA rules to fill our needs

### Tools used

* TryHackMe
* Linux CLI

## Flags

* NO FLAGS TODAY 

### Practical portion
1. Start the target machine
2. Read about YARA rules and what they are used for.
3. Enter the terminal
4. CMD nano to enter Text editor
5. Copy the existing YARA rule and make some changes to the strings and conditions
6. Save the rule by using the ctrl x to exit text editor
7. Asks if we would like to save yes
8. Name the text document
9. Back on main screen of the terminal
10. We type yara -rs (for recursive search) /home/ubuntu/TBFC_Simple_MZ_Detect /home/ubuntu
11. We are displayed with matching .jpg's with messages displayed
12. We organize those messages based on the numbers behind the .jpg title
13. Message we find is Find me in hopsec island.

## Takeaways from todays room

Todays room was one that I really enjoyed it was cool to see how we can set rules to analyze meta data to find a message. I was excited to use the command line one of the first things that I learned when I started this journey into Cyber security. The CLI can be a bit overwhelming at first but I have enjoyed the challenge of learning the proper syntax and formatting for commands.

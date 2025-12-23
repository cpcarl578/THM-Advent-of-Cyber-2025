# Advent of Cyber Day 19-ICS/Modbus-Claus for Concern

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

* How SCADA (Supervisory Control and Data Acquisition)systems monitor industrial processes
* What PLC's (Programmable Logic Controllers) do in automation
* How the Modbus protocol enables communication between industrial devices
* How to identify compromised system configurations in industrial systems
* Techniques for safely remediating compromised control systems
* Understanding protection mechanisms and trap logic in ICS environments

### Skills Learned/Lessons learned

* How insecure industrial control systems can be
* Intro into ICS and Modbus systems

### Tools used

* Platform-TryHackMe
* Linux CLI
* Python Scripts

## Flags

* THM{eGgMas0v3r}

### Practical portion

1. Start Attacker machine
2. Start target machine
3. Run an nmap scan on ports 22,80,502 and the Attacker machine IP
4. Those ports are shown as open
5. Navigate to the IP address specified to view the security cameras for the factory
6. Run pip3 install pymodbus==3.6.8
7. Run command python3
8. Connect to the PLC on port 502
9. Stopped and read through the rest of the steps
10. Picked back up on running command nano reconnaissance.py
11. Copied a script and saved that in the GNU editor
12. Run the script python3 reconnaissance.py
13. output is a recon report showing some of the damage on the system
14. Run command nano restore_christmas.py
15. Copy script and save that buffer
16. Run python3 restore_christmas.py
17. The script runs and disables the issues that we found in the reon report
18. We are presented with the Flag at the end of the script THM{eGgMas0v3r}
19. We have completed todays room

## Takeaways from todays room

Today was an eye opener for me. I got to see how vulnerable some Industrial control systems are. Some of the logic behind these systems is if it isn't broke don't fix it. These are essential systems and they need to be protected from attackers as if they are attacked they could shut down a full factory. This was a little out of my realm but it was something interesting to learn about.

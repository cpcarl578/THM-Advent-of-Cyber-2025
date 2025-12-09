# Advent of Cyber Day 4 AI in Security- Old sAInt nick

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

- How can AI be used as an assistant in cyber security for different tasks, domains and roles.
- Using an AI assistant to solve the various tasks that we may encounter in cyber security
- Considerations surrounding the use of AI, particularly in cyber secuirty





### Skills Learned/Lessons learned

- How dangerous SQL injections exploits are
- Use of AI for analyzing a  large log file
- Challenges and considerations of using AI in cybersecurity
- Generation of Python scripts using CLI
- Use of AI models and how they relate to Cybersecurity

### Tools Used

- Platform used to learn- TryHackMe

### Practical Portion

1. Launch the Attack machine and target machine via THM's attackbox
2. Launch web interface on attackbox
3. Input "http://10.65.140.245" into the search bar
4.  Read instructions on how we are going to interact with the AI for todays challenges
5. Use Van SolveIT to Generate  the python script for the vulnerabilty within the web app of todays Advent of Cyber web application
6.Read about the existing  SQL Vulnerablity and why it exists and how we are going to exploit it. 
7. Open Terminal  
8.  Use PWD in CLI to Print the working directory to see what directory we are in
8.  On terminal, use nano script.py to create a file
9.  Paste the script that  Van SolveIT Generated into GNU on terminal
10.  Change the IP address to the IP of the attack box which was "http://10.64.142.151"
11.  Save the file by using Ctrl + X and exit
12.  Respond Y to GNU asking if we want to buffer/save the file and hit enter
13. Back on the Main portion of the CLI we type nano script.py to open the file we just created and confrim that the username and password are setup properly by confirming username is "alice" or 1=1 -- -" (common for SQL injection) confirm password is "test"
14. exit back out of GNU
15. Run Script python3 script.py
16. Script was run sucessfully and we have exploited the vuln sucessfully and we captured [FLAG:THM{SQLI_EXPLOIT]
17. Go to target IP address and log in using alice or "1=1 -- -" 
18. confirm we can login and access the [FLAG:THM{SQLI_EXPLOIT]
19. Stage three of using Van SolveIT-Blue team
20. Ask AI to analyse logs and it has detected a breach in the system and outputs an analysis of the code
21. AI tells us that a malicous code was executed.
22. AI explains the malicious code with helpful insights.
23. Stage 4 of using Van SolveIT Software
24. The Software assistant analyses sources code from the exploit with helpful insights and things that we need to change or make better.
25. Complete the showcase of Van SolveIT and presented with the Flag THM{AI_MANIA}




## Takeaways

Today I learned about how dangerous SQL injections can be and used the attack box to exploit a SQL injection on a vulnerable target. This was a great introduction to the power of AI in cybersecurity. Learned about some  of the cautions and considerations that need to be taken  when using AI in Cyber security. One of the cautions when using AI in cybersecurity is to "Trust but verify" using AI, AI can make mistakes and you need to be aware of that and Verify its output. 


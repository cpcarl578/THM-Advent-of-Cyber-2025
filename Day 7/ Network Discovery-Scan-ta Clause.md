# Day 7 Network Discovery-Scan-ta Clause

![Static Badge](https://img.s hields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

1. Learn the basics of network service discovery with Nmap
2. Learn core network protocols and concepts
3. Apply the knowledge learned to find a way back into the server



### Skills Learned/Lessons learned ( A lot of todays topics were things I am still learning as I am a beginner so I will hit some basic highlights)

- Netcat
- Nmap exposure
- Identifying ports that are open by using Nmap

### Tools Used

- Platform used to learn- TryHackMe
- nmap
- Netcat

## Flags

- THM{4ll_s3rvice5_discovered}
 
### Practical Portion

1. Start Attacker machine
2. Start target machine
3. Open terminal and type nmap 10.66.154.32
4. After running that command we are alerted that there are two open ports we can choose from.
5. If we knew the username and password we could select SSH but we do not so we are going to go with the HTTP
6. We go to the IP address listed for the website and take a look and we need to find three keys to unlock the website for today
7. Enter nmap -p- --script=banner 10.66.154.32 and run that command 
8. Wait until we get a message that nmap is finished scanning and we review the results
9. Several open ports are shown and take a look at them.
10. Following along with todays video and access FTP in anonymous mode
11. We are into the server and we type LS for List systems 
12. Find one of the keys may be listed in this directory.
13. ftp asks what to do next type "get tbfc_qa_key1 - "
14. CLI shows the hidden key "3aster_"
15. use "!" to exit the ftp
16. out of the ftp and back to the learning module/instructions for today
17. Read about using the universal tool called Netcat
18. Use the command "nc -v 10.66.154.32 25251" and run that 
19. Displayed with all of the correct information that we are connected to the custom app
20. Use "GET KEY" command and faced with a message saying "not armed" may have had a possible syntax typo and copy and paste the correct syntax
21. presented with key "15_th3_"
22. use CTRL+C to exit netcat
23. clear the terminal so we start with a fresh screen on the CLI
24. Read more about TCP and UDP ports 
25. Back on CLI run the command "nmap -sU 10.66.154.32"
26. Presented with a message that port 53 is open
27. Read about using the command "dig" which is used to perform advanced DNS queries
28. Run command "dig @10.66.154.32 TXT key3.tbfc.local +short"
29. Presented with key3 "n3w_xm45"
30. go to the ip address in firefox "10.66.154.32"
31. Access  the admin console by using the prior keys we found previously.
32. Run command on Admin console "ss -tunlp"
33. Show data for listening ports and TCP and UDP ports 
34. looking for the 3306 port we want to see the database information so we are going to be using the mysql program
35. Run command mysql -D tbfcqa01 -e "show tables;"
36. Shown two tables, one of the tables is called flags 
37. Run command mysql -D tbfcqa01 -e "select * from flags;"
38. Displayed with the flag THM{4ll_s3rvice5_discovered}
39. Answer questions on THM and complete the room 



## Takeaways

Todays room was looking into open ports on a network using Nmap and Ncat via the CLI. After this room I have a very basic understanding of using Nmap and Ncat and after the Advent of cyber I am sure that my continued learning will delve even deeper into these tools. I am a visual learner and up until the AOC started I have only read about these tools so it was nice to  visually see how they function and why they are important.

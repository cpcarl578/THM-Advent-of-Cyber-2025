# Advent of Cyber Day 24-Explotation with cURL-Hoperation

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

* Understand what HTTP requests and responses are at a high level.
* Use cURL to make basic requests (using GET) and view raw responses in the terminal.
* Send POST requests with cURL to submit data endpoints.
* Work with cookies and sessions in cURL to maintain login state across requests.

### Skills Learned/Lessons learned

* Loops
* How to manually brute force something with specific parameters

### Tools used

* Platform-TryHackMe
* Linux CLI

## Flags

* THM{curl_post_success}
* THM{session_cookie_master}
* THM{user_agent_filter_bypassed}

### Practical portion

1. Launch the attacker machine
2. Start the target machine
3. Open the terminal and run command "curl http://IP ADDRESS/
4. create a text document named passwords.txt
5. Add required passwords to the document per instructions
6. Make a bash loop using touch command to make a file "loop.sh"
7. Run the command chmod +x loop.sh to add execute to permissions to this file
8. We enter the command ls -la to double check the permission we added is there
9. Enter command ./loop.sh to run the loop we just created
10. We found the password that worked which is secretpass
11. Read and run the commands in the reading about the user agent
12. Run the command "curl -X POST -d "username=admin&password=admin&submit=login" http://IPADDRESS/post.php
13. Receive a flag as we are successfully logged in Flag- THM{curl_post_success}
14. Question asks to make a request to /cookie.php endpoint with username admin and password admin save the cookie and receive the flag THM{session_cookie_master}
15. Bypass the agent by running the command "curl -i -A "TBFC" http://IPADDRESS/agent.php
16. Receive the flag THM{user_agent_filter_bypassed}

## Takeaways from todays room

I enjoyed todays room learning about curl. I have used curl a little bit here and there outside of the AOC challenge. I am going to continue learning curl after the AOC is done I know the list of things that I need to learn is ever growing. I did attempt the side quest but am a bit lost on this.I Hope everyone enjoyed these writeups I know I was not always on time getting them posted but I enjoyed learning to write one and using GitHub to post them. Lastly Merry Christmas!

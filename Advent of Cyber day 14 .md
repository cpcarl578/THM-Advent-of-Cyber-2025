# Advent of Cyber Day 14-Container Security

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

* Learn How Docker and containers work,container engine, images,and layers
* Explore docker runtime concepts such as sockets, daemon api and common container escape/ privilege escalation vectors
* Apply skills learned from todays reading to investigate image layers, escape a container, escalate privileges.

### Skills Learned/Lessons learned

* Basic use of escalation of a container.
* Learning how docker differs from a VM.

### Tools used

* TryHackMe
* Docker
* Linux CLI

## Flags

*THM{DOCKER_ESCAPE_SUCCESS}

### Practical portion

1. Start the attacker machine
2. Start the target machine
3. Read through todays learning
4. Run command docker ps to see what services are running
5. Run command docker exec -it uptime-checker sh
6. Than run command ls -la /var/run/docker.sock to check socket access
7. Run command docker ps again
8. Run command docker exec -it deployer bash
9. We are now logged into the web app
10. Run command whoami to confirm we are logged in as deployer
11. Run sudo /recovery_script.sh
12. Message displayed that the container is restarting
13. Recovery is complete
14. Run ls command
15. Notice that there is a .txt file
16. Run command cat flag.txt
17. Receive flag "THM{DOCKER_ESCAPE_SUCCESS}
18. Find secret code on port 5002 (DeployMaster2025)

## Takeaways from todays room

Todays room was a little overwhelming at first as I am not familiar with docker or containers quite yet. I did enjoy escaping the container as part of todays challenge as it made me feel a sense of accomplishment. Learning about the different uses for containers was also interesting as I have read about using containers before but have never seen it or experienced it hands on.

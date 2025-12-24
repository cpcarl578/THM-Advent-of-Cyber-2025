# Advent of Cyber Day 20-Race Conditions-Toy to The World

## Objectives

* Understand what race conditions are and how they can affect web applications
* Learn how to identify and exploit race conditions in web requests
* How concurrent requests can manipulate stock or transaction values
* Explore simple mitigation techniques to prevent race condition vulnerabilities

### Skills Learned/Lessons learned

* More Burpsuite
* Understand why Race conditions are important

### Tools used

* Platform-TryHackMe
* Burpsuite

## Flags

* THM{WINNER_OF_R@CE007}
* THM{WINNER_OF_Bunny_R@ce}

### Practical portion

1. Launch the attacker machine
2. Launch the Target machine
3. Launch Firefox and ensure foxyproxy burpsuite profile is running
4. Open burpsuite and ensure that intercept is off
5. Go back to Firefox and login to the specified address
6. Select the product we want to purchase and checkout
7. Back in burpsuite find the process checkout and send that to repeater
8. Find the process in the repeater tab and add a tab group
9. We name a group called cart
10. Duplicate the tab 19 times
11. Go to repeater and send group in parallel (last byte sync)
12. Send group parallels launches all 19 requests to the server simultaneously
13. We go to the webapp and find that the stock has gone negative and two flags are displayed
14. THM{WINNER_OF_R@CE007} is the first flag
15. THM{WINNER_OF_Bunny_R@ce}

## Takeaways from todays room

start here

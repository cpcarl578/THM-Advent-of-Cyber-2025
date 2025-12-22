# Advent of Cyber Day 16-Forensics-Registry Furensics

## Objectives

* Understand what windows registry is and what it contains
* Dive deep into Registry hives and root keys
* Analyze Registry hives and root keys
* Learn registry forensics and investigate through the registry explorer tool

### Skills Learned/Lessons learned

Exposure and hands on skills using registry forensics to see where a application was installed.

### Tools used

* TryHackMe
* Windows Registry explorer

## Flags

* No flags today

### Practical portion

1. Start the attack machine
2. Open and look at the Registry hives
3. Open Registry editor to see what we have listed in the hives
4. Open Registry explorer
5. Load the registry hive system while holding shift so we get a clean hive state
6. Go to ROOT\ControlSet001\Control\ComputerName\Computername
7. Find DISPATCH-SRV01
8. Have a basic understanding of how Registry explorer works
9. Load the Software Hive into registry explorer
10. Looking for a application that was installed on dispatch-srv01 after 10-21 is when abnormal activity began
11. Look for uninstalled applications
12. Find Dronemanager updater
13. Load NTUSER.DAT hive
14. Search for the path to the uninstall of dronemanager updater
15. Look for windows NT and move to Compatibility assistant
16. Find store
17. Multiple values here but we know we are looking for  where the user would have launched the application Dronemanager updater
18. Find Path
19. What value was added for this application to main persistence on startup
20. Find a path with --background for the dronemanager updater

## Takeaways from todays room

Today took me a little longer to complete as I have never used registry explorer. After getting some basic knowledge I was able to answer the rooms questions for today. This was interesting to see how you can do forensics on a specific application. I was impressed to see that you can drill down to some of the first things that are done after installing an application and investigate some logs to see uninstall data. After the AOC I will be returning to the forensics rooms as this was pretty interesting to me.

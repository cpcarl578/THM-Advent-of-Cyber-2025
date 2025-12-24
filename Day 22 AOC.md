# Advent of Cyber Day 22-C2 Detection-Command & Carol

## Objectives

* Convert a PCAP to Zeek logs
* Use RITA to analyze Zeek logs
* Analyze the output of RITA

### Skills Learned/Lessons learned

* Basic understanding of RITA
* Info level of understanding PCAPS

### Tools used

* Platform-TryHackMe
* RITA

## Flags

* No Flags today

### Practical portion

1. Launch the target machine
2. Open the terminal
3. Parse  the PCAPS into logs
4. Run the command rita import --logs ~zeek_logs/asyncrat/ --database asyncrat
5. RITA has parsed and analyzed our data
6. run the command rita view asyncrat
7. RITA terminal pops up and we can see detailed information about threats and events
8. Review the two events that we see and inspecting the second one with virus total we see some red flags literally
9. Repeat the above steps to look at the data for the challenge for today
10. Answer the questions by analyzing RITA
11. End todays room

## Takeaways from todays room

The hands on portion of todays lesson was interesting to me. I was able to see how RITA works and the detections it can provide and alert the user to. It will score connections by severity and can even give a count as to how many times the connection occurred and the source of the connection.

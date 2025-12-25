# Advent of Cyber Day 23-AWS Security-S3cret Santa

![Static Badge](https://img.shields.io/badge/Linux-yellow?logo=linux&logoColor=white&labelColor=black&color=yellow)

## Objectives

* Learn the basics of AWS accounts
* Enumerate the privileges granted to an account, from an attackers perspective
* Familiarize myself with AWS CLI

### Skills Learned/Lessons learned

* AWS CLI
* How AWS systems format and function

### Tools used

* Platform-TryHackMe
* AWS

## Flags

* THM{more_like_sir_cloudbane}

### Practical portion

1. Launch the target machine
2. Open the terminal
3. Use command aws sts get-caller-identity
4. We are displayed with credentials in the CLI
5. Run the command "aws iam list-users"
6. View the printed output of the command we ran and review the users information
7. See what inline policies are availible for the username information we have by running "aws iam list-user-policies --user-name sir.carrotbane
8. We are presented with an inline policy
9. Run command aws iam list-attached-user-policies --user-name sir.carrotbane to see what attached policies to the account there are.
10. Output shows no attached user policies to this account in particular.
11. Check the username to see if it is part of a group by running command aws iam list-groups-for-user --user-name sir.carrotbane
12. output displayed shows that this particular user is not apart of any groups.
13. Checking to see what permissions are granted to this user by using "aws iam get-user-policy --policy-name SirCarrotbanePolicy --user-name sir.carrotbane and we are presented with all of the access to enumerate all different kinds of users
14. We find one that is sts assume role
15. Find out what other roles we can assume and we find bucketmaster and we are going to see what kind of permissions they have
16. No other attached policy
17. 3 different actions assigned to this role, Listallbuckets,listbuckets, and getobjectsfromeastersecrets
18. we use the command aws sts assume-role --role-arn arn:aws:iam::123456789012:role/bucketmaster --role-session-name TBFC
19. We are presented with the credentials including access key,secret access key, and session token.
20. After assuming the roll we do some investigating and find a document that we download to the VM.
21. Presented with the flag THM{more_like_sir_cloudbane}
22. End todays room.

## Takeaways from todays room

Today was pretty straightforward and I got to use one of my favorite newfound skills which is the command line. Using AWS in the command line was easy to understand. The exploitation portion was very easy given the correct information and user access roles.

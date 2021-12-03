# What is Mimikatz: The Beginner’s Guide

notes taken from <https://www.varonis.com/blog/what-is-mimikatz/>

## What is Mimikatz

Mimikatz is an open-source application that allows users to view and save authentication credentials like Kerberos tickets. Benjamin Delpy continues to lead Mimikatz developments, so the toolset works with the current release of Windows and includes the most up-to-date attacks.

Attackers commonly use Mimikatz to steal credentials and escalate privileges: in most cases, endpoint protection software and anti-virus systems will detect and delete it. Conversely, pentesters use Mimikatz to detect and exploit vulnerabilities in your networks so you can fix them.

## What can Mimikatz do

1. Pass-the-Hash
2. Pass-the-Ticket
3. Over-Pass the hash (Pass the Key)
4. Kerberos Golden Ticket
5. Kerberos Silver Ticket
6. Pass-the-Cache

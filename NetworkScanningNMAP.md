# What is a Port Scanner and How Does it Work?

notes taken from the above named article: <https://www.varonis.com/blog/port-scanning-techniques/>

## Port Scanners

Port scanners are valuable tools that at the most basic level check to see if a port is open, closed or filtered.  Integral in problem solving connection issues.

## How Does a Port Scanner Operate?

Port scaners send a network request to connect and record the response helping network engineers diagnose network issues or application connectivity.

## What is a Port?

Ports are virtual locations where networking communication starts and ends. There are a total of 131,082 ports divided in half for TCP and UDP.

Internet Assigned Numbers Authority (IANA) reserves the first 1023 as well known ports to keep them standardized.

1024 - 49151 are used for services and applications and 49152 and above are free to use.

## Port Scanning Basics

A port scanner sends a TCP or UDP network packet and asks the port about their current status. The three types of responses are below:

1. Open, Accepted: The computer responds and asks if there is anything it can do for you.
2. Closed, Not Listening: The computer responds that “This port is currently in use and unavailable at this time.”
3. Filtered, Dropped, Blocked: The computer doesn’t even bother to respond.

## Types of Port Scanning

1. Ping Scan "The simplest port scans are ping scans. A ping is an Internet Control Message Protocol (ICMP) echo request – you are looking for any ICMP replies, which indicates that the target is alive."

2. TCP Halp Open "SYN packets request a response from a computer, and an ACK packet is a response. In a typical TCP transaction, there is an  SYN, an ACK from the service, and a third ACK confirming message received."

3. TCP Connect "basically the same as the TCP Half-Open scan, but instead of leaving the target hanging, the port scanner completes the TCP connection."

4. UDP "For example, if you want to know if a DNS server is up, you would send a DNS request. For other UDP ports, the packet is sent empty."

5. Stealth Scanning "When you send a port scan with a packet and the FIN flag, you send the packet and not expecting a response. If you do get an RST, you can assume that the port is closed. If you get nothing back, that indicates the port is open. Firewalls are looking for SYN packets, so FIN packets slip through undetected."

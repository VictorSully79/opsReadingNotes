# What is an SMB Port? Ports 445 and 139 Explained
notes taken from above name article: <https://www.upguard.com/blog/smb-port>

SMB protocol allows computers to talk to each other.

Although it has evolved over time the CIFS or Common Internet File System is a specific implementation of SMB that enables file sharing.

History:
- SMB 1.0 (1984)
- Samba (1992)
- CIFS (1996)
- NQ (1998)
- Netsmb (2004)
- SMB 2.0 (2006)
- Tuxera SMB (2009)
- Likewise (2009)
- SMB 2.1 (2010)
- SMB 3.0 (2012)
- MoSMB (2012)
- SMB 3.02 (2014)
- SMB 3.1.1 (2015)

## What are Ports 139 and 445

139 and 445 are the ports that SMB use.

139 is used by smb dialects that communicate of NetBIOS

445 is used post Windows 2000 on top of a TCP stack allowing for communication over the internet.
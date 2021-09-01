# Active Directory

notes taken from: <https://www.cyberark.com/what-is/active-directory/>

Active Directory is an indentity management servcie for Windows domain networks and is included with most Microsoft Windows Server operating systems.

Active Directory Services:

- Active Directory Domain Services (AD DS) – the core Active Directory service used to manage users and resources.

- Active Directory Lightweight Directory Services (AD LDS) – a low-overhead version of AD DS for directory-enabled applications.

- Active Directory Certificate Services (AD CS) – for issuing and managing digital security certificates.

- Active Directory Federation Services (AD FS) – for sharing identity and access management information across organizations and enterprises.

- Active Directory Rights Management Services (AD RMS) – for information rights management (controlling access permissions to documents, workbooks, presentations, etc.)

A server running Active Directory Domain Service is called a domain controller. There is usually one or more backups to the domain controller for resiliency.

Active Directory stores information about the network users and all of the other resouces in a structure consisting of domains, trees and forests.

- A domain is a collection of objects (e.g. users, devices) that share the same Active Directory database. A domain is identified by a DNS name like company.com.

- A tree is a collection of one or more domains with a contiguous namespace (they have a common DNS root name like marketing.company.com, engineering.company.com, and sales.company.com).

- A forest is a collection of one or more trees that share a common schema, global catalog, and directory configuration—but aren’t part of a contiguous namespace. The forest typically serves as the security boundary for an enterprise network.


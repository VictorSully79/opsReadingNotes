# Network Address Translation (NAT)

notes taken from the above named article at: <https://www.geeksforgeeks.org/network-address-translation-nat/>

NAT is the process of translating one or more local IP addresses int Global IP addresses and vice versa to gain Internet access to local hosts. It also provides translation of port numbers i.e. masks the port numbers of the host with another port number, in the packet that will be routed to the destination. Then makes the corresponding entries of IP addresses to port numbers in the NAT table. Generally done at the router or firewall level. 

## NAT working

Packets entering or leaving the local network are translated from global to local IP and vice versa.

If NAT runs out of addresses the packets can not be sent.

## Types of Addresses

- NAT inside and outside addresses: *Inside refers to the addresses which must be translated. Outside refers to the addresses which are not in control of an organization. These are the network Addresses in which the translation of the addresses will be done.*

- Inside local address: *An IP address that is assigned to a host on the Inside (local) network. The address is probably not an IP address assigned by the service provider i.e., these are private IP addresses. This is the inside host seen from the inside network.*

- Inside global address: * IP address that represents one or more inside local IP addresses to the outside world. This is the inside host as seen from the outside network.*

- Outside local adress: *This is the actual IP address of the destination host in the local network after translation.*

- Outside global address: *This si the outside host as seen from the outside network. It is the IP address of the outside destination host before translation.*


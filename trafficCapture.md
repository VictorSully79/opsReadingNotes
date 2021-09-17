# How to capture network traffic ? SPAN vs TAP

notest taken from the above named article: <https://accedian.com/blog/capture-network-traffic-span-vs-tap/>

## Port Mirroring

Port Mirroring forwards a copy of the incoming and outgoing packets from one or several ports of a switch to another port.

Advantages:

- Low cost

- Can be configured remotely through IP or Console port.

- The only way to capture intra-switch traffic

- A good way to capture traffic on several ports at once.

Drawbacks:

- Not adequate for fully utilized full-duplex links

- Filters out physical errors

- Impact on the switch's CPU

- Can alter the timeing of the frame

- SPAN has a lesser priority than port to port data transfer. 

## Network TAP

- Hardware device which can passively capture traffic on a network.

Advantages:

- No risk of dropped packets.

- Monitoring of all packets

- Provides full visibility, including congestion situations.

Drawbacks:

- The device may require two listening interfaces on the analysis device

- Costly

- No visibility on intra-switch traffic

- Not appropriate for the observation of a narrow tgraffic range.  
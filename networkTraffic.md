# Understanding Network Data Delivery: Layers 2 and 3 of the OSI Model

Notes taken from the above named article: <https://www.comptia.org/blog/layers-2-and-3-osi-model>

The (OSI) model stands for Open Systems Interconnections model. Represented by 7 layers and describes how computers communicate.  

7 Layers:

  1. Physical
  2. Data Link
  3. Network
  4. Transport
  5. Session
  6. Presentation
  7. Application

Layer 2 is split into 2 parts, MAC sub layer and data link sub layer

MAC (or physical) addressing provides an effective method of moving data across a small community of computing devices where routing traffic between multiple communities is not required.

Uniformity is an important characteristic and includes placing both addresses for the data sender as well as the data recipient. Figure 2 below provides an example of an Ethernet II frame.

Layer 3 provides the structure relating to how data can be efficiently transferred from one network to another. layer 3 requires the creation of an outside envelope over the layer 2 frame, that includes the layer 3 address of the sender of the packet, along with the layer 3 address of the recipient.

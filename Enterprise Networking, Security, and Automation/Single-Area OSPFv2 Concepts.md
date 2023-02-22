# 1.1 OSPF Features and Characteristics
Open Shortest Path First (OSPF)


OSPF is a link-state routing protocol that was developed as an alternative for the distance vector Routing Information Protocol (RIP). RIP was an acceptable routing protocol in the early days of networking and the internet. However, the RIP reliance on hop count as the only metric for determining best route quickly became problematic. Using hop count does not scale well in larger networks with multiple paths of varying speeds. OSPF has significant advantages over RIP in that it offers faster con
vergence and scales to much larger network implementations.

OSPF is a link-state routing protocol that uses the concept of areas. A network administrator can divide the routing domain into distinct areas that help control routing update traffic. A link is an interface on a router. A link is also a network segment that connects two routers, or a stub network such as an Ethernet LAN that is connected to a single router. Information about the state of a link is known as a link-state. All link-state information includes the network prefix, prefix length, and cost.

### 1.2.2 Types of OSPF Packets

Link-state packets are the tools used by OSPF to help determine the fastest available route for a packet. OSPF uses the following link-state packets (LSPs) to establish and maintain neighbor adjacencies and exchange routing updates. Each packet serves a specific purpose in the OSPF routing process, as follows:

* Type 1: Hello packet - This is used to establish and maintain adjacency with other OSPF routers.
* Type 2: Database Description (DBD) packet - This contains an abbreviated list of the LSDB of the sending router and is used by receiving routers to check against the local LSDB. The LSDB must be identical on all link-state routers within an area to construct an accurate SPF tree.
* Type 3: Link-State Request (LSR) packet - Receiving routers can then request more information about any entry in the DBD by sending an LSR.
* Type 4: Link-State Update (LSU) packet - This is used to reply to LSRs and to announce new information. LSUs contain several different types of LSAs.
* Type 5: Link-State Acknowledgment (LSAck) packet - When an LSU is received, the router sends an LSAck to confirm receipt of the LSU. The LSAck data field is empty.
The table summarizes the five different types of LSPs used by OSPFv2. OSPFv3 has similar packet types.
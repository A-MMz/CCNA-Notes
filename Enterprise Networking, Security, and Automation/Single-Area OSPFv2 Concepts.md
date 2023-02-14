# 1.1 OSPF Features and Characteristics
Open Shortest Path First (OSPF)


OSPF is a link-state routing protocol that was developed as an alternative for the distance vector Routing Information Protocol (RIP). RIP was an acceptable routing protocol in the early days of networking and the internet. However, the RIP reliance on hop count as the only metric for determining best route quickly became problematic. Using hop count does not scale well in larger networks with multiple paths of varying speeds. OSPF has significant advantages over RIP in that it offers faster con
vergence and scales to much larger network implementations.

OSPF is a link-state routing protocol that uses the concept of areas. A network administrator can divide the routing domain into distinct areas that help control routing update traffic. A link is an interface on a router. A link is also a network segment that connects two routers, or a stub network such as an Ethernet LAN that is connected to a single router. Information about the state of a link is known as a link-state. All link-state information includes the network prefix, prefix length, and cost.

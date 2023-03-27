# RipProtocol
RIP (Routing Information Protocol) is a distance-vector routing protocol that is used to exchange routing information between routers within a small- to medium-sized network. 
RIP is a simple protocol that uses a hop count as its metric to determine the best path to a destination network.
RIP routers periodically broadcast their entire routing table to their neighbors. 
Each router updates its own routing table with the information it receives from its neighbors, and then broadcasts its updated routing table to its own neighbors.
The hop count metric used by RIP represents the number of routers that a packet must pass through to reach a destination network. 
The maximum hop count that RIP supports is 15, which means that RIP is not well-suited for large networks with many hops.
RIP routers perform a split horizon with poison reverse to prevent routing loops. 
Split horizon means that a router does not advertise a route back to the neighbor from which it learned that route. Poison reverse means that when a route is no longer available, a router advertises that route to its neighbors with an infinite metric to prevent them from sending traffic to a destination that is no longer reachable.
One of the advantages of RIP is its simplicity. RIP routers are easy to configure and require minimal administrative overhead. RIP is also supported by many different vendors and hardware platforms.

However, RIP has several limitations. Because RIP updates are broadcasted periodically, there can be significant delays in reacting to changes in the network topology. Additionally, the hop count metric used by RIP can result in suboptimal routing decisions in networks with many hops. Finally, RIP does not support authentication, which makes it vulnerable to attacks from malicious users who could inject false routing information into the network.

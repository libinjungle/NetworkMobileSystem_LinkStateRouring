# NetworkMobileSystem_LinkStateRouring


This assignment is part of Seattle project. It will illustrate an important network routing strategy called Link State routing. 

In this assignment, Seattle nodes will take an initial connectivity map of nodes. They will then implement and run Dijkstra's shortest 
path algorithm to build their routing tables. Finally, nodes will forward packets using their routing table. This routing table is weighted since it is based on the latency between two nodes.

Initially, a connectivity map (neighboriplist.txt) of nodes was built as a starting point. It then reads this map and build connections on it. The main function 
used at this step is waitforconn(srcip, srcport, makeconn). It essentially spawns a socket thread to handle the incoming connection.
Since node are connected with each other, directly or implicitly, packet sending from one node can be received by all other nodes. This is tested in the flood connectivity step. Since there are 13 states in neighboriplist.txt, each node should receive 13 connectivity messages. If that is the case, the connectivity information is flooded successfully. 

Next, weighted routing table is built on each node using Dijkstra's shortest path mechanism is used to build routing table based on weight.

Finally, I use the weighted routing table on each node to forward packets.

I registered 9 hosts which spread all over the world.

NOTE: Code is writen based on repy, a restricted python version which provides safety when running on remote hosts.

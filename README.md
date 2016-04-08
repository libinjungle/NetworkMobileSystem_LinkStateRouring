# NetworkMobileSystem_LinkStateRouring

I registered 9 hosts which spread all over the world.
This assignment is part of Seattle project. It will illustrate an important network routing strategy called Link State routing. 

In this assignment, Seattle nodes will take an initial connectivity map of nodes. They will then implement and run Dijkstra's shortest 
path algorithm to build their routing tables. Finally, nodes will forward packets using their routing table. This routing table is weighted
since it is based on the latency between two nodes.

Initially, a connectivity map (neighboriplist.txt) of nodes was built as a starting point. It then reads this map and build connections on it. The main function 
used at this step is waitforconn(srcip, srcport, makeconn). It essentially spawns a socket thread to handle the incoming connection.






NOTE: Code is writen based on repy, a restricted python version which provides safety when running on remote hosts.

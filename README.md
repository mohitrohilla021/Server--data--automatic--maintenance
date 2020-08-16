# Server--data--automatic--maintenance

We have created a few classes to simulate a server that's taking connections from the outside and then a load balancer that ensures that there are enough servers to serve those connections.
To represent the servers that are taking care of the connections, we'll use a Server class. Each connection is represented by an Id; that could, for example, be the IP address of the computer connecting to the server. For our simulation, each connection creates a random amount of load in the server, between 1 and 10.
New server gets added automatically to ensure that the average load of all servers is not more than 50%.

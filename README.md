# Server--data--automatic--maintenance
A database server is a server which uses a database application that provides database services to other computer programs or to computers, as defined by the client–server model.

Database management systems (DBMSs) frequently provide database-server functionality, and some database management systems (such as MySQL) rely exclusively on the client–server model for database access (while others e.g. SQLite are meant for using as an embedded database).

Users access a database server either through a "front end" running on the user's computer – which displays requested data – or through the "back end", which runs on the server and handles tasks such as data analysis and storage.

In a master-slave model, database master servers are central and primary locations of data while database slave servers are synchronized backups of the master acting as proxies.

Most database applications respond to a query language. Each database understands its query language and converts each submitted query to server-readable form and executes it to retrieve results.

We have created a few classes to simulate a server that's taking connections from the outside and then a load balancer that ensures that there are enough servers to serve those connections.

To represent the servers that are taking care of the connections, we'll use a Server class. Each connection is represented by an Id; that could, for example, be the IP address of the computer connecting to the server. For our simulation, each connection creates a random amount of load in the server, between 1 and 10.

New servers get added automatically to ensure that the average load of all servers is not more than 50%.



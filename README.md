# Distributed-Word-Count-using-MapReduce-in-Go
I use a master-worker architecture that  includes three parts: the master server, the slave client, and the mapper and reducer functions.

The master server listens for incoming connections from slave machines, stores them on a map, and sends commands to the slaves. The slave client connects to the master server, sends its ID, and waits for commands. Once a command is received, the slave reads a file, performs a word count, and sends the result back to the master. The mapper and reducer functions are used to perform the map and reduce phases of the algorithm.

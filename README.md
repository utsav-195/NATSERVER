# NATSERVER
This is a simple implementation of NAT Server using java.
It is basically used to maintain privacy of the clients connected to it by changing the source IP address(client's IP) to it's(NAT sevrer's) own IP address.

Steps to implement the code:

1. Compile the natServer code and execute(run) it. The server will start accepting clients on the given port number.

2. Compile the natClient code and run it. It will get connected to the server. 

*Note: We need minimum 2 clients to implement this concept. So, in another window again repeat step 2.

*Note: In this implementation the maximum number of clients has been restricted to 10(static value).

3. After executing the client side code, we need to enter the name of each client that will be registered with the server along with the IP address.

*Note: IP address of the client is allocated by the server side here(for ease of implementation).

4. If the client wants to send some data/message to all the others clients in the network, directly enter the message.

5. If the client wants to send some data/message to any one particular client,
Syntax: @client_name message
Example. @client2 HelloFromTheOtherSide

6. The server will receive the data from the client, which includes the source IP, data and the destination IP.

*Note: If the data is to be sent to all clients in the network, the destination IP would be 'broadcast', else it will be the destination IP of the client to which the data is forwarded.

7. The server changes the source IP address to it's own IP address before forwarding the packets to the respective destinations.

8. To disconnect from the network, client has to enter '/quit'.

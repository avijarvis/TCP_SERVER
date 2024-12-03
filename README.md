Step-by-step Explanation:

net.Listen("tcp", ":8080"): The server starts listening for connections on port 8080.
listener.Accept(): The server accepts an incoming connection.
go handleConnection(conn): Each connection is handled in a separate function (handleConnection) so the server can continue accepting new connections.
fmt.Fprintln(conn, "Hello from TCP server"): Sends a simple message to the client.


How the Server Code Works:
Start Listening: The server listens on port 8080 for any incoming TCP connections.
Accept Connections: When a client tries to connect, the server accepts it.
Handle Each Connection: Each connection is handled by a separate part of the code so that the server can continue listening for more connections.
Send and Receive Data: The server sends a greeting message to the client and prints out information about the connection.

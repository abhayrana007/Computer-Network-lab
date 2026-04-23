------------------------------------------------------------
HTTP SIMULATION LOG & ANALYSIS
------------------------------------------------------------

TEST 1: ICMP CONNECTIVITY
- PC0 to 192.168.1.1 -> Success (4/4 packets)
- PC1 to 192.168.1.1 -> Success (4/4 packets)

TEST 2: HTTP REQUEST CAPTURE (Simulation Mode)
- Protocol: HTTP
- Method: GET
- Destination: 192.168.1.1:80
- Source: 192.168.1.2:1025
- Status: Client sent SYN (TCP Handshake) -> SYN/ACK -> ACK -> GET Request.

TEST 3: HTTP RESPONSE CAPTURE
- Response Code: 200 OK
- Content-Type: text/html
- Server: Cisco Packet Tracer HTTP Service
- Status: Page rendered successfully on client browser.

------------------------------------------------------------
OBSERVATION:
The simulation confirms that HTTP is a stateless protocol that relies on 
a reliable TCP connection. The 3-way handshake was visible prior to the 
actual transmission of the HTTP GET request.
------------------------------------------------------------

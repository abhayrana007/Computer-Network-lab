TEST CASE 01: Successful Webpage Retrieval
- Action: Enter 'http://192.168.1.1' in PC0 Browser.
- Expected: 'Welcome to Cisco Packet Tracer Web Server!' header appears.

TEST CASE 02: HTTP Service Availability
- Action: Turn 'HTTP' service OFF on the server and attempt access.
- Expected: Browser displays "Host Name Unresolved" or "Connection Timeout."

TEST CASE 03: Protocol Inspection
- Action: In Simulation Mode, click on the HTTP packet.
- Expected: Inbound PDU shows "HTTP Data: GET / index.html HTTP/1.1".

TEST CASE 04: Simultaneous Access
- Action: Initiate web requests from PC0 and PC1 at the same time.
- Expected: Both PCs successfully render the page independently.

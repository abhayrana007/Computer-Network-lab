TEST CASE 01: Verify TCP 3-Way Handshake
- Action: Initiate HTTP traffic from PC2.
- Observation: Event list must show [SYN], [SYN-ACK], and [ACK] before [HTTP] data.

TEST CASE 02: UDP Header Analysis
- Action: Send TFTP data from PC0 to PC1.
- Observation: Inspect PDU details; verify a small 8-byte header and no sequence numbers.

TEST CASE 03: SCTP Association
- Action: Generate SCTP traffic.
- Observation: Verify the "Association" state and check for multi-stream tags in the PDU.

TEST CASE 04: Congestion Simulation
- Action: Flood the switch with excessive ICMP and UDP traffic.
- Observation: Notice TCP window size scaling down (Flow Control) while UDP remains constant.

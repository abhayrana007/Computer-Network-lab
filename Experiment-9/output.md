------------------------------------------------------------
SIMULATION RESULTS: TRANSPORT LAYER COMPARISON
------------------------------------------------------------

SCENARIO 1: TCP TRANSMISSION (PC2 to PC3)
- Connection Setup: 3-Way Handshake Successful.
- Acknowledgment: Every segment acknowledged.
- Error Handling: Packet dropped at Router -> Retransmission triggered.
- Result: 100% Data Integrity; Moderate Latency.

SCENARIO 2: UDP TRANSMISSION (PC0 to PC1)
- Connection Setup: None. First packet is Data.
- Acknowledgment: None.
- Error Handling: Packet dropped at Router -> No retransmission.
- Result: High Speed; Data Loss observed under congestion.

SCENARIO 3: SCTP TRANSMISSION (PC4 to PC5)
- Connection Setup: 4-Way Handshake (INIT, INIT-ACK, COOKIE-ECHO, COOKIE-ACK).
- Feature Test: Multi-homing simulation (switching between two interfaces).
- Result: High Availability; Robust connection.

------------------------------------------------------------
Final Conclusion: 
TCP is essential for accuracy (Web, Email), UDP for speed (Streaming, VoIP), 
and SCTP for specialized signaling and high-availability systems.
------------------------------------------------------------

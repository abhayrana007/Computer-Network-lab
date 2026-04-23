TEST CASE 01: Simultaneous Transmission (Pure ALOHA)
- Action: Send 3 PDUs from PC0, PC1, and PC2 at T=0.
- Result: Collision observed at Hub; all packets failed.

TEST CASE 02: Slotted Synchrony (Slotted ALOHA)
- Action: Send PDUs from PC0 and PC1.
- Result: Collision only if both start at the exact same slot start-time.

TEST CASE 03: Carrier Sensing (CSMA/CD)
- Action: PC0 starts transmission; PC1 attempts to start 0.1ms later.
- Result: PC1 senses the medium is busy and waits (Deferring).

TEST CASE 04: RTS/CTS Mechanism (CSMA/CA)
- Action: Laptop0 sends data to Access Point.
- Result: Observe RTS control frame before the actual Data frame.

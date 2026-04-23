TEST CASE 01: Window Full Scenario
- Action: Set Window Size = 3. Send 5 packets.
- Result: Sender transmits Packets 0, 1, and 2, then pauses until ACK 0 is received.

TEST CASE 02: Piggyback Verification
- Action: Initiate a bidirectional file transfer (Simulated).
- Result: Inspect Inbound PDU on Sender. Verify the ACK field is non-zero within a Data frame.

TEST CASE 03: Performance under Latency
- Action: Increase link delay to 50ms.
- Result: Throughput remains high due to the Sliding Window, unlike Stop-and-Wait which drops significantly.

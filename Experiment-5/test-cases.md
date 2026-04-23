Test Case 1: Ideal Channel (No Loss)
- Run all three protocols.
- Expect: GBN and SR to have significantly higher packet delivery rates than Stop-and-Wait.

Test Case 2: Single Packet Drop
- Manually "Delete" a packet in simulation mode.
- GBN Expectation: Notice the sender jumping back to the dropped frame number.
- SR Expectation: Notice the receiver buffering subsequent packets while waiting for the retransmission.

Test Case 3: ACK Timeout
- Simulate a lost ACK from Receiver to Sender.
- Expect: Sender retransmission after the T-out timer expires.

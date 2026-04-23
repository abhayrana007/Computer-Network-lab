Test Case 1: Standard ICMP Ping
- Expected: 100% Success, No CRC Errors.

Test Case 2: Manual Bit Flip (Conceptual)
- Action: Modify PDU bit in Simulation Note.
- Expected: CRC Checksum mismatch at Receiver.

Test Case 3: Block Code Redundancy
- Action: Calculate Parity for 4-bit data.
- Expected: Detection of single-bit flip in the simulation log.

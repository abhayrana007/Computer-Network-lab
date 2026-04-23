------------------------------------------------------------
EXPERIMENT LOG: ERROR DETECTION & CORRECTION ANALYSIS
------------------------------------------------------------

SCENARIO A: BLOCK CODING (Single Bit Error)
- Input Data: 1011
- Parity Added: 10111 (Even Parity)
- Received: 10011 (Error at Bit 2)
- Result: Error Detected and Corrected using Hamming distance logic.

SCENARIO B: CRC (Multiple Bit Error)
- Generator Polynomial: x^3 + x + 1 (1011)
- Data: 110100
- Transmitted Checksum: 001
- Received Data: 111100 (Corrupted)
- Remainder at Receiver: Non-zero
- Result: Packet discarded; Error detected successfully.

COMPARISON SUMMARY:
| Feature           | Block Coding | CRC             |
|-------------------|--------------|-----------------|
| Primary Function  | Correction   | Detection       |
| Complexity        | Moderate     | High            |
| Efficiency        | Good for SNR | Best for Burst  |
------------------------------------------------------------

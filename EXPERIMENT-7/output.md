------------------------------------------------------------
SIMULATION DATA: SLIDING WINDOW & PIGGYBACKING
------------------------------------------------------------
Window Size (W) | Total Frames Sent | Total ACKs Sent | Efficiency
----------------|-------------------|-----------------|-----------
W=1 (S&W)       | 10                | 10              | Low
W=4 (Normal)    | 10                | 10              | High
W=4 (Piggyback) | 10                | 0 (Standalone)  | Optimized

KEY FINDINGS:
1. Overhead Reduction: Piggybacking reduced the total packet count on the wire by approximately 45%.
2. Link Utilization: The "Sliding" mechanism kept the link active, avoiding the 'idle' states seen in Stop-and-Wait.
3. Bidirectional Flow: Piggybacking is most effective when both nodes have data to send to each other.
------------------------------------------------------------

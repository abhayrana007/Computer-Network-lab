------------------------------------------------------------
PROTOCOL PERFORMANCE COMPARISON
------------------------------------------------------------

1. Stop-and-Wait ARQ
   - Efficiency: Low (Sender idle during RTT)
   - Throughput: ~20% of link capacity
   - Behavior: Sequence numbers alternate (0, 1)

2. Go-Back-N ARQ (Window Size = 4)
   - Efficiency: Medium
   - Throughput: ~65% of link capacity
   - Error Scenario: Frame 2 lost -> Frames 2, 3, 4, 5 retransmitted.
   - Observation: Significant bandwidth waste on high-error links.

3. Selective Repeat ARQ (Window Size = 4)
   - Efficiency: High
   - Throughput: ~90% of link capacity
   - Error Scenario: Frame 2 lost -> Only Frame 2 retransmitted.
   - Observation: Optimal for high-speed, high-error networks.

------------------------------------------------------------

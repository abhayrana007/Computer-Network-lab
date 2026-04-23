------------------------------------------------------------
PERFORMANCE ANALYSIS REPORT
------------------------------------------------------------
Protocol        | Collision Rate | Efficiency (S) | Complexity
----------------|----------------|----------------|-----------
Pure ALOHA      | Very High      | 18.4%          | Low
Slotted ALOHA   | High           | 36.8%          | Medium
CSMA/CD         | Moderate       | High           | Medium
CSMA/CA         | Low            | Very High      | High

OBSERVATIONS:
1. ALOHA (Hub-based): Collisions occur frequently as traffic load increases. 
   In Pure ALOHA, even a partial overlap destroys both packets.
2. CSMA/CD: Improved throughput significantly by sensing the carrier; 
   however, collisions still occur due to propagation delay.
3. CSMA/CA: The use of Inter-Frame Spacing (IFS) and Backoff timers 
   successfully avoided most collisions in the wireless simulation.
------------------------------------------------------------

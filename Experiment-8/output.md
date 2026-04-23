------------------------------------------------------------
PROTOCOL VERIFICATION LOG
------------------------------------------------------------

1. ARP ANALYSIS (PC0 -> PC1)
   - Step: Ping 192.168.1.3
   - Packet Type: ARP Request (Broadcast)
   - Target MAC: FF:FF:FF:FF:FF:FF
   - Result: PC1 replied with Unicast MAC; PC0 updated ARP Cache.

2. DHCP DORA SEQUENCE (PC0)
   - [DISCOVER] PC0: "Need IP"
   - [OFFER] Server: "Use 192.168.1.2"
   - [REQUEST] PC0: "I'll take 192.168.1.2"
   - [ACK] Server: "Confirmed. Lease starts now."

3. IPv6 CONNECTIVITY
   - Command: ping 2001:db8::2
   - Protocol: ICMPv6
   - Status: 0% Loss. Neighbor Discovery (NDP) successful.

------------------------------------------------------------

TEST CASE 01: Dynamic Allocation
- Action: Change PC0 from 'Static' to 'DHCP' mode.
- Expected: PC0 receives 192.168.1.2, Subnet 255.255.255.0, and Gateway 192.168.1.1.

TEST CASE 02: ARP Cache Clearing
- Action: Run 'arp -d' on PC0, then Ping PC1.
- Expected: Observe the initial 'Request' packet in Simulation Mode before the ICMP Echo.

TEST CASE 03: IPv6 Global Unicast
- Action: Ping between 2001:db8::1 and 2001:db8::2.
- Expected: Connectivity established without a DHCPv6 server (using SLAAC or Static).

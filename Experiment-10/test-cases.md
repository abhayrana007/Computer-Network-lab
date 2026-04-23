TEST CASE 01: Standard DNS Forward Lookup
- Action: On PC0, ping 'test.com'.
- Expected: PC0 resolves 'test.com' to 192.168.1.3 and receives ICMP replies.

TEST CASE 02: Negative DNS Query
- Action: On PC0, nslookup 'unknown.com'.
- Expected: Server returns "Can't find unknown.com: Non-existent domain."

TEST CASE 03: Record Modification
- Action: Manually change 'example.com' mapping on the Server.
- Expected: PC1 reflects the new IP immediately upon next query.


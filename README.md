# pkt_gen
packet generator for TCP/IP protocols.

So far the following protocols are supported.

1. Ethernet
2. ARP
3. QinQ
4. VLAN
5. MACsec
6. IPV4
7. ICMP
8. UDP


## How to Run ?

The release is based on AARCH64 Apple architecture. Works only on AARCH64 architecture.
Future release targeted to X86-86.

```bash
sudo ./packet_gen -f packet_gen.json
```

Currently only one protocol can be enabled at a time to generate packets.


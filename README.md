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
9. TCP

It can also replay pcap files as well.

Look at `packet_gen.json` on fine tuning the packet generation.

## How to Run ?

The release is based on AARCH64 Apple architecture.

To run on AARCH64 machines,

```bash
sudo ./packet_gen -f packet_gen.json
```

To run on X86-64 machines, install `qemu-aarch64-static` and run

```bash
sudo qemu-aarch64-static ./packet_gen -f packet_gen.json
```


Currently only one protocol can be enabled at a time to generate packets.


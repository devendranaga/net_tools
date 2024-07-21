# pkt_gen
packet generator for TCP/IP protocols.

# Disclaimer

The tool is kept here for learning and testing purposes only. It is not intended to be used for
malicious or harmful purposes directly or indirectly. The author of the tool are not liable
or responsible for any damages caused by the tool results.

# Description

More description about how to use the tool is [here](https://devnaga.substack.com/p/packet-generator).

So far the following protocols are supported.

1. Ethernet
2. ARP
3. QinQ
4. VLAN
5. Double tagged VLANs
6. MACsec
7. IPV4
8. ICMP
9. UDP
10. TCP

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


Currently only one protocol can be enabled at a time to generate packets. The tool cannot be used to send multiple protocols at a time.

## New features:

### v0.1.0000

Below are the new features since last release:

1. Double tagged VLANs
2. TCP with flags
3. along with sending the generated packets, the tool now logs them into a pcap file


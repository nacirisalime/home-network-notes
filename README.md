# Home Network Setup

Small project to document my home network and practice some networking basics for my FISI preparation.

## Setup
- **Router:** FRITZ!Box (192.168.1.1) Handles DHCP and local routing
- **PC:** 192.168.1.100 (Ethernet cable, static IP for convenience)
- **Other devices:** Dynamic IPs assigned via router DHCP

![Network Diagram](./home_network.png)

## Useful commands I use for testing
```bash
# Check PC network configuration
ipconfig /all

# Check if I can reach the router
ping 192.168.1.1

# Verify that DNS is resolving domain names
nslookup google.com

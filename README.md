# Home Network Setup

Small project to document my home network and practice some networking basics for my FISI preparation.

## Setup
- Router: FRITZ!Box (192.168.1.1) -> Handles DHCP and local routing
- PC: 192.168.1.100 (Ethernet cable, static IP for convenience)
- Other devices: Dynamic IPs assigned via router DHCP
- Testing tools: CLI tools (cmd) and PowerShell

## Useful commands I use for testing
- ipconfig /all
- ping 192.168.1.1
- nslookup google.com

## Notes / Things to remember
- Difference between static IP (manual) and DHCP (automatic from router).
- The gateway is needed to leave the local network and reach the internet.

  ## Real world Troubleshooting & Log
  When setting up static Ip assignments and testing local connectivity, here is the routine I follow when diagnosing connection issues:
 - Physical & Layer 2: Verify link speed and cable status
 - Ip Configuration (ipconfig /all): Ensure the correct subnet mask (255.255.255.0) and Default Gateway (192.168.1.1) are assigned
 - Gateway Ping: Check if local packets reach the router. If it fails the issue is strictly inside the local network
 - External DNS Check (nslookup google.com): To test if domain name works. if "ping 8.8.8.8" works but domain names fail it is a DNS issue

  ## Next step or Future Improvements 
 - Experiment with local DNS filtering or a dedicated home server setup

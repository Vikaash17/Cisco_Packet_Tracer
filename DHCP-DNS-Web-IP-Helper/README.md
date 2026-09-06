# DHCP-DNS-Web-IP-Helper

This is a Cisco Packet Tracer lab based on **DHCP, DNS, Web Server, and IP Helper**.

The main aim of this lab is to understand how these services work together when the DHCP server and client are on different networks.

## What I configured

- DHCP Server
- DNS Server
- Web Server
- Router
- `ip helper-address`
- IP configuration for PCs
- Connectivity testing

## Network

The topology contains:

- 1 Router
- 2 Switches
- 1 DHCP Server
- 1 DNS Server
- 1 Web Server
- Multiple PCs

## IP Addresses

| Device      | IP Address                |
| ----------- | ------------------------- |
| Router      | 192.168.1.1 / 192.168.2.1 |
| DHCP Server | 192.168.2.2               |
| DNS Server  | 192.168.2.3               |
| Web Server  | 192.168.2.4               |

## IP Helper

The `ip helper-address` command is used on the router to forward DHCP requests from one network to the DHCP server located on another network.

```text
ip helper-address 192.168.2.2
```

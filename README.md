# Linux Networking Cheatsheet

This repository contains Linux networking commands, troubleshooting steps, and practical notes.

## Topics
- IP addressing and routing
- DNS debugging
- TCP/UDP testing
- Port scanning
- Firewall basics
- SSH troubleshooting
- Tools: ping, curl, ss, netcat, tcpdump

## Author
Adithya Gowda
---

# Advanced Networking Troubleshooting

## Check Open Ports
ss -tulnp
netstat -tulnp

## Test Port Connectivity
nc -zv <host> <port>

## Trace Route
traceroute <domain>
mtr <domain>

## DNS Lookup
nslookup <domain>
dig <domain>

## Check Listening Process
lsof -i :80

## Check Network Interfaces
ip a
ip route

## Check Firewall Rules
sudo iptables -L -n -v
sudo ufw status

## Packet Capture
sudo tcpdump -i eth0

# Advanced Networking Troubleshooting Cheatsheet

## Check Open Ports
ss -tulnp
netstat -tulnp

## Test Port Connectivity
nc -zv <host> <port>

## DNS Debugging
dig <domain>
nslookup <domain>

## Trace Network Path
traceroute <domain>
mtr <domain>

## Check Listening Process
lsof -i :80

## Check Routing Table
ip route

## Packet Capture
sudo tcpdump -i eth0

## Check Firewall
sudo iptables -L -n -v
sudo ufw status

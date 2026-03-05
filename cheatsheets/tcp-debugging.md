# TCP Debugging Cheatsheet

## Check Active Connections
ss -t
netstat -tn

## Check Listening Ports
ss -tulnp

## Test TCP Port
nc -zv <host> <port>

Example:
nc -zv google.com 443

## Capture TCP Packets
sudo tcpdump -i eth0 tcp

## Trace Network Path
traceroute <host>

## Check SYN / Connection Attempts
sudo tcpdump 'tcp[tcpflags] & tcp-syn != 0'

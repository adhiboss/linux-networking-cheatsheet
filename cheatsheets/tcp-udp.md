# TCP vs UDP Cheat Sheet

## TCP (Transmission Control Protocol)
### Features
- Connection-oriented (3-way handshake)
- Reliable delivery
- Ordered packets
- Retransmission on loss
- Flow control + congestion control

### Common Uses
- HTTP/HTTPS
- SSH
- FTP
- SMTP/IMAP email

### Testing TCP (netcat)
Server:
```bash
nc -l -p 8080

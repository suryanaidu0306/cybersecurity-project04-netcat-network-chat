# Project 4 — Netcat Network Chat

## Objective
Build a simple text chat between two terminal windows using Netcat and TCP on the same Linux computer.

## Tools Used
- Ubuntu Linux
- Netcat OpenBSD
- TCP/IP
- Bash terminal

## How It Works
One terminal listens for an incoming TCP connection. The second terminal connects to the listener using the loopback address `127.0.0.1` and port `12345`. Text typed into either connected terminal is sent to the other.

## Commands

**Terminal 1 — Server**
```bash
nc -lv 127.0.0.1 12345
```

**Terminal 2 — Client**
```bash
nc 127.0.0.1 12345
```

## Test
1. Start the server.
2. Connect the client.
3. Send a message from the client.
4. Reply from the server.
5. Record the result in `output.txt`.

## Learning Outcomes
- Client-server communication
- TCP connections
- Port numbers
- Netcat usage
- Local network troubleshooting

## Safety
This exercise binds to the loopback address, so it is intended for communication on the same computer. Use Netcat listeners only on systems and networks you are authorized to use.

## Author
Surya Naidu

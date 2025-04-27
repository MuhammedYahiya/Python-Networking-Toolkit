
# Networking Tools – Python Socket Programming

## About

This project provides basic networking tools built with Python's socket programming and threading. It includes:

- **Netcat Clone**: A remote command execution, file upload, and shell access tool.
- **TCP Client**: A simple client for sending HTTP requests and receiving responses.
- **Multithreaded TCP Server**: A server that can handle multiple client connections.

## Files Included

| File           | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `netcat.py`    | Python-based Netcat clone with command shell, execution, and file upload features. |
| `tcp_client.py`| A simple TCP client that connects to a server and sends a basic HTTP request. |
| `tcp_server.py`| A multithreaded TCP server that accepts and responds to multiple client connections. |

## How to Run

### Netcat Tool (`netcat.py`)

#### Start server (listen for shell):

```bash
python netcat.py -t [your_IP] -p 5555 -l -c
```

#### Connect to server:

```bash
python netcat.py -t [server_IP] -p 5555
```

#### Upload a file:

```bash
python netcat.py -t [server_IP] -p 5555 -l -u=myfile.txt
```

### TCP Client (`tcp_client.py`)

```bash
python tcp_client.py
```
(Sends a GET request to Google and prints the response.)

### TCP Server (`tcp_server.py`)

```bash
python tcp_server.py
```
(Listens on port 9998 and responds with "ACK" when it receives a message.)

## Requirements

- Python 3.x
- No external libraries needed (only standard libraries: socket, threading, subprocess, etc.)

## Key Concepts

- **Socket Programming**
- **TCP Communication**
- **Multithreading**
- **Command Execution Over Network**
- **File Transfer Over TCP**

## License

This project is created for educational purposes only. Use responsibly.

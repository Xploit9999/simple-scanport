### DESCRIPTION

It's a simple scan port for tcp and udp connections.

### USAGE
Usage options [ -s -p -r -P ]

    -s = Enter the server(s), if they are a group, put them inside quotes, e.g., "srv1 srv2"
    -p = Enter the port(s), if it's a group, put them inside quotes, e.g., "80 22 23"
    -r = Port range, enter the range of ports in this format, e.g., 80-120
    -P = specify protocol to use (tcp, udp)

```vim
# Single host and single port:

$ ./scanport -s 192.168.1.4 -p 22 -P tcp

# Multiple hosts and multiple ports:

$ ./scanport -s "192.168.1.4 192.168.1.6" -p "53 21" -P udp

# Range ports on a host:

$ ./scanport -s 192.168.1.4 -r 20-40 -P tcp 
```

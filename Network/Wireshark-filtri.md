##Wireshark Filter by IP

```
ip.addr == 10.10.50.1

```
Filter by Destination IP

```
ip.dest == 10.10.50.1

```
Filter by Source IP

```
ip.src == 10.10.50.1

```
Filter by IP range

```
ip.addr >= 10.10.50.1 and ip.addr <= 10.10.50.100

```
Filter by Multiple Ips

```
ip.addr == 10.10.50.1 and ip.addr == 10.10.50.100

```
Filter out IP address

```
!(ip.addr == 10.10.50.1)

```
Filter subnet

```
ip.addr == 10.10.50.1/24

```
Filter by port

```
tcp.port == 25

```
Filter by destination port

```
tcp.dstport == 23
```

Filter by ip address and port

```
ip.addr == 10.10.50.1 and Tcp.port == 25
```

Filter by URL

```
http.host == “host name”
```

Filter by time stamp

```
frame.time >= “June 02, 2019 18:04:00”
```

Filter SYN flag

```
tcp.flags.syn == 1


tcp.flags.syn == 1 and tcp.flags.ack == 0
```

Wireshark Beacon Filter

```
wlan.fc.type_subtype = 0x08
```

Wireshark broadcast filter

```
eth.dst == ff:ff:ff:ff:ff:ff
```

WiresharkMulticast filter

```
(eth.dst[0] & 1)

```
Host name filter

```
ip.host = hostname

```
MAC address filter

```
eth.addr == 00:70:f4:23:18:c4
```

RST flag filter

```
tcp.flags.reset == 1
```

# Network+ Notes

## OSI and TCP/IP Models

| OSI              | TCP/IP          |
| ---------------- |---------------- |
| 7 - Application  | 4 - Application |
| 6 - Presentation |                 |
| 5 - Session      |                 |
| 4 - Transport    | 3 - Transport   |
| 3 - Network      | 2 - Internet    |
| 2 - Data Link    |                 |
| 1 - Physical     | 1 - Network Interface (Link)|

* Please Do Not Take Salami Pizza Away

## Cabling Notes
### Coax Cabling
- RG = (Radio Grade)
- RG-58 - 50 Ohms
- RG-59 - 75 Ohms
- RG-6 - 75 Ohms

Connectors
- F-type: Threaded
- BNC: Locking pin

## Ethernet Standards
- Max Length for utp ~100m
- Cat rating is based on twists per inch

| Name | Speed | Notes |
|-|-|-|
| Cat 3 | 10 Mbps | Obsolete |
| Cat 5 | 100 Mbps ||
| Cat 5e | 100 Mbps to 1000 Mbps | Replaced Cat5 |
| Cat 6 | 1 Gbps | 10Gb for ~55 m |
| Cat 6a | 10 Gbps ||
| Cat 7 | 10 Gbps | Shielded connectors and twisted pairs |

#### 10 Mbps
| TBase Standard | Cable Type | Speed | Max Distance | Extra Info |
|-|-|-|-|-|
| 10BaseT | Cat 3 or better |10 Mbps | 100 m | Max 1024 Nodes |
#### 100 Mbps
| TBase Standard | Cable Type | Speed | Max Distance | Extra Info |
|-|-|-|-|-|
| 100BaseT4 |Cat 3 | 100 Mbps | 100 m | replaced by Tx \ 1024 nodes \ uses all 4 utp pairs |
| 100BaseTx | Cat 5e | 100 Mbps | 100 m | 1024 nodes \ only uses 2 utp pairs \ known as 100BaseT |
| 100BaseFX | multimode | 100 Mbps | 2 Km | 1024 nodes \ |
#### Gigabit
| TBase Standard | Cable Type | Speed | Max Distance | Extra Info |
|-|-|-|-|-|
| 1000BaseCX | TwinAX | 1 Gbps | 25 m | Copper Standard|
| 1000BaseSX | multimode | 1 Gbps | 500 m ||
| 1000BaseLX | single mode | 1 Gbps | 5 km ||
| 1000BaseT | Cat 6 | 1 Gbps |100 m ||
#### 10 Gigabit / SONET (Internet Backbone)
| TBase Standard | Cable Type | Speed | Max Distance | Extra Info |
|-|-|-|-|-|
| 10GBaseT | Cat 6 or Cat 6a | 10 Gbps | 6 - 55m \ 6a - 100m ||
| 10GBaseSR | multimode | 10 Gbps | 26 - 400m | SW/EW/LW |
| 10GBaseLR | single mode | 10 Gbps | 10 km | 1310 nm \ SW/EW/LW |
| 10GBaseER | single mode | 10 Gbps | 40 km | 1550 nm \ SW/EW/LW |

## Subnetting Info

### Subnets must be all 1's followed by all 0's
### Bit Math
(128, 64, 32, 16, 8, 4, 2, 1)

Determines local or long distance calls.
```
(255.255.255.0)
Each block is 8 bits
(11111111.11111111.11111111.00000000)
```

### Classless Inter-Domain Routing (CIDR)
CIDR (/24)

Where 255's exist, network ID numbers cannot be changed.
192.168.1.xxx/24 = 254 hosts, 0 and 255 not used.

### Network ID
192.168.1.0
(no host ID can end in .0 or .255)

## Networking Commands
| Windows | Linux/Mac | Purpose | Flags |
|-|-|-|-|
| ipconfig | ifconfig | show network info | -a (show all NIC info) |
| tracert | traceroute | show hops | |
| ping | ping | test network connection | |
| netstat | netstat | show all active connections | -n (only ip addresses) -b (executable) -o (process id) -a (active ports) -r (local routing table) |
| nbtstat | N/A | show NetBios info | |
| arp ||||
| nslookup ||||

## Important Port Numbers
| Port Number | Function |
| ----------- | -------- |
| 20 | ftp (file transfer protocol) |
| 21 | ftp |
| 22 | ssh (secure shell) |
| 23 | telnet (telephone network) |
| 25 | smtp |
| 53 | dns (domain name service) |
| 80 | http (hyper text transport protocol) |
| 110 | pop3 |
| 115 | sftp (secure ftp) |
| 123 | ntp (network time protocol) |
| 143 | imap |
| 161 | snmp (simple network management protocol) |
| 220 | imap3 |
| 443 | https (secure http) |
| 465 | TLS / STARTTLS(old) |
| 587 | STARTTLS(new) |

## RJ45 Connection wiring

|Connector Pin #   | 468A Color       | 468B  Color     |
| ---------------- | ---------------- |---------------- |
|8|Brown|Brown|
|7|Brown/White|Brown/White|
|6|Orange|Green|
|5|Blue/White|Blue/White|
|4|Blue|Blue|
|3|Orange/White|Green/White|
|2|Green|Orange|
|1|Green/White|Orange/White|

```
Switch Green and Orange. A = Split Oranges, B = Split Greens
```


## Connector Identification

## Virtual Local Area Networks (VLAN)
Default VLAN is 1, CompTIA 0

Setup in Managed Switches.
Switch ports assigned by technician.
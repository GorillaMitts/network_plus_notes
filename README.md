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


## Important Port Numbers
| Port Number | Function |
| ----------- | -------- |
|80|http|
|443|https|
|25|smtp|
|22|ssh|
|23|telnet|

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
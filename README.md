# wifi

## Introduction

Display wireless network information.

## Dependencies

- netctl
- iw
- ip
- hostname
- wget

## Usage

### Print wifi strength

```
wifi
```

### Connect to a network

This uses *netctl* profiles to connect to a network. As a result, the name
specified on the command line must be the name of the profile's file under
*/etc/netctl*.
```
wifi -c profile
```

### Disconnect from the network

The following command will disconnect from the currently connected network.
```
wifi -d
```

### Print extra wifi information

The following command will print out: IPv4 address, ISP name, Services, City,
Region, and Country.
```
wifi -i
```

### Print your private IP address

```
wifi -p
```

### Print your public IP address

```
wifi -P
```

### Scan all wifi networks

The following command will print out wifi networks and their strengths near your
computer.
```
wifi -S
```

For verbose information on all detected wifi networks, run the following command.
```
wifi -F
```

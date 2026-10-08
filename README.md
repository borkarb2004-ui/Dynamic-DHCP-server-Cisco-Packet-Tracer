# Dynamic-DHCP-server-Cisco-Packet-Tracer

Dynamic DHCP Server configuration using Cisco Router and Packet Tracer

## Objective

To configure a Dynamic Host Configuration Protocol (DHCP)
server on a Cisco router and automatically assign IP addresses
to client PCs.

## Topology

Router → Switch → PCs

## Network Details

Network: 192.168.10.0/24
Router/Gateway: 192.168.10.1
DHCP Range: 192.168.10.11 - 192.168.10.254
DNS Server: 8.8.8.8

## Technologies

- Cisco Packet Tracer
- Cisco IOS
- DHCP
- IPv4
- LAN Networking

## Configuration

ip dhcp excluded-address 192.168.10.1 192.168.10.10

ip dhcp pool LAN
network 192.168.10.0 255.255.255.0
default-router 192.168.10.1
dns-server 8.8.8.8

## Verification

show ip dhcp binding
show ip dhcp pool
show running-config

## Testing

Clients successfully received IP addresses
automatically from the DHCP server.

Ping connectivity was also verified.

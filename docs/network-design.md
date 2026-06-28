# Network Design

Network Mode

Bridged Adapter

Reason

A bridged network more closely resembles an enterprise LAN by allowing the virtual machines to exist as independent devices on the guest network.

Current Addressing

Server01

192.168.10.10

Client01

192.168.10.20

Client02

192.168.10.30

Subnet

255.255.255.0 (/24)

Gateway

Guest Network Router

DNS

Currently:
Router DNS

Planned:
Server01 (Domain Controller)

Firewall

Windows Defender Firewall enabled.

Inbound rules will be configured rather than disabling the firewall.
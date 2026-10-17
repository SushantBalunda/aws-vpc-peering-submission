# Network Architecture

The project contains two VPCs connected through AWS VPC Peering.

## Network layout

- VPC A: `10.10.0.0/16`
  - Public subnet: `10.10.1.0/24` — Bastion
  - Private subnet: `10.10.2.0/24` — App-A
- VPC B: `10.20.0.0/16`
  - Private subnet: `10.20.1.0/24` — App-B

## Traffic flow

Laptop → Bastion → App-A or App-B
App-A ↔ VPC Peering ↔ App-B

Both application instances use private IPv4 addresses.

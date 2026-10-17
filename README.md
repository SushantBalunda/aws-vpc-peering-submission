# aws-vpc-peering-submission
# AWS VPC Peering — EWB Student Project

## Overview

This project implements a private network connection between two Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering.

The objective is to demonstrate private IPv4 connectivity between two EC2 application servers while keeping both application servers private and using a bastion host for administration.

## Architecture

- **VPC A:** `10.10.0.0/16`
- **VPC B:** `10.20.0.0/16`
- **Public subnet A:** `10.10.1.0/24`
- **Private subnet A:** `10.10.2.0/24`
- **Private subnet B:** `10.20.1.0/24`

### EC2 Instances

| Instance | Private IPv4 |
|---|---|
| Bastion | `10.10.1.10` |
| App-A | `10.10.2.10` |
| App-B | `10.20.1.10` |

## Technologies

- Amazon Web Services (AWS)
- Amazon VPC
- VPC Peering
- Amazon EC2
- Route Tables
- Security Groups
- SSH and ICMP
- GitHub and Markdown

## Project Objectives

1. Create two VPCs with non-overlapping CIDR ranges.
2. Configure public and private subnets.
3. Create and activate a VPC peering connection.
4. Configure forward and return routes.
5. Restrict inbound traffic using security groups.
6. Access private instances through a bastion host.
7. Verify connectivity using ping and SSH.
8. Demonstrate controlled failure and recovery.
9. Document the architecture, configuration and results.

## Repository Structure

- `architecture/` — Network architecture diagrams.
- `screenshots/` — Evidence captured during actual execution.
- `documentation/` — Configuration and troubleshooting notes.
- `report/` — Final project report.

## Implementation Status

- [ ] VPCs and subnets created
- [ ] Route tables configured
- [ ] Security groups configured
- [ ] EC2 instances launched
- [ ] VPC peering activated
- [ ] Forward and return routes configured
- [ ] Private connectivity verified
- [ ] Controlled failure and recovery demonstrated
- [ ] Final report completed
- [ ] AWS resources cleaned up

## Security Notes

- Application servers must not have public IPv4 addresses.
- SSH access must be restricted to approved sources.
- Private keys, passwords, access tokens and AWS credentials must never be committed to this repository.
- Screenshots and test results must reflect actual execution.

## Evidence and Results

Screenshots, resource IDs, connectivity results and the final report will be added after the implementation is completed.

## Learning Outcomes

This project aims to develop practical understanding of VPC networking, IP addressing, routing, network security, SSH access and troubleshooting in AWS.

## Disclaimer

This repository documents an educational lab project. AWS usage may incur charges. Resources should be removed after testing, and actual results should be recorded before claiming completion.

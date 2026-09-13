# Containerlab + Ansible: DHCP + Network Automation lab

## Overview
This repository contains an automated network lab using **Containerlab** and **Ansible**. It demonstrates Infrastructure as Code (IaC) principles by automatically deploying an Alpine Linux DHCP server and configuring network endpoints.

## Tech Stack
* **Container Engine:** Docker
* **Network Emulation:** Containerlab
* **Automation:** Ansible (YAML / Jinja2)
* **OS / Network Devices:** Alpine Linux (`dnsmasq` and client device), Arista cEOS (access switch)

## Topology
* `dhcp-server`: Alpine Linux container running `dnsmasq`
* `sw-access-1`: Access layer Arista cEOS switch passing DHCP traffic
* `client-01`: Client node receiving dynamic IP assignments

## Quick Start

### 1. Prerequisites
Ensure you have Docker, Containerlab and Ansible installed
```bash
sudo containerlab version
ansible --version

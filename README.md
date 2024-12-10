# CrowdSec Ansible Setup

This repository contains Ansible playbooks for setting up **CrowdSec** in a **controller-agent** architecture. The setup includes configurations for the CrowdSec controller, agent, and various bouncers like **firewall (iptables)** and **nginx**.

## Requirements

- Ansible version 2.9 or later
- Access to the controller and agent machines
- Linux distributions with CrowdSec support (Debian/Ubuntu)

## Setup Instructions

1. Configure your hosts in the `inventory/hosts.ini` file.
2. Run the playbooks to set up the controller and agent:
   ```bash
   ansible-playbook -i inventory/hosts.ini playbooks/controller_setup.yml
   ansible-playbook -i inventory/hosts.ini playbooks/agent_setup.yml

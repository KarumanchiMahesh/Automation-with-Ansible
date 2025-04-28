# Flask App with HAProxy Load Balancer

This repository contains an Ansible playbook to deploy a simple Flask application and an HAProxy load balancer across three servers (devA, devB, devC) in a private network. 

## Files:
- **hosts**: The Ansible inventory file containing the details of the hosts.
- **site.yaml**: The Ansible playbook for deploying Flask app and HAProxy.
- **haproxy.cfg.j2**: The configuration template for HAProxy.

## Setup Instructions:
1. Clone this repository.
2. Set up servers (HAproxy, devA, devB, devC, bastion).
3. Configure SSH keys and update the `hosts` file with your private IP addresses.
4. Run the Ansible playbook:

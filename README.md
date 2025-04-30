# Flask App with HAProxy Load Balancer Deployment

This repository contains the Ansible playbook and configurations to deploy a Flask application behind an HAProxy load balancer.

## Requirements

- 5 Ubuntu 20.04 servers:
  - bastionNSO (bastion host)
  - HAproxy (load balancer)
  - devA, devB, devC (backend servers)
- SSH key configured for access via bastion host

## Files

1. `hosts` - Ansible inventory file
2. `site.yaml` - Main Ansible playbook to deploy the Flask app with HAProxy Load Balancer
3. `haproxy.cfg.j2` - HAProxy configuration template
4. `test_deployment.yaml` - To test the deployment 

## Deployment Steps

1. Clone this repository
2. Configure SSH to use bastion host as jump host
3. Run the playbook: 
```
ansible-playbook -i hosts site.yaml
```
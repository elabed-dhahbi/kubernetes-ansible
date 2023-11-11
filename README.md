Kubernetes Cluster Setup with HAProxy and Keepalived
This repository contains an Ansible playbook for setting up a high-availability Kubernetes cluster on Ubuntu. The cluster includes master nodes, a worker node, and HAProxy nodes with Keepalived for load balancing.

Prerequisites
Ensure the following collections are installed:

ansible.posix version 1.5.4
community.general version 8.0.1
community.kubernetes version 2.0.1
kubernetes.core version 2.4.0
Inventory Setup
Node Configuration:

| Node Type | Hostname  | IP Address    |
|-----------|-----------|---------------|
| Master    | master1   | 192.168.1.190 |
| Master    | master2   | 192.168.1.191 |
| Master    | master3   | 192.168.1.192 |
| Worker    | worker1   | 192.168.1.193 |
| HAProxy   | haproxy1  | 192.168.1.194 |
| HAProxy   | haproxy2  | 192.168.1.195 |
| Elastic IP| N/A       | 192.168.1.199 |

Adjust the inventory to match your environment.

Usage
Customize the variables as needed and run the playbook to set up the cluster.


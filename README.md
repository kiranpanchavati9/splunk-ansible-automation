# Splunk Ansible Automation

This repository contains Ansible playbooks and roles for installing, configuring, and managing a distributed Splunk Enterprise environment.

It is designed to work with infrastructure created by the related Terraform project.

## Purpose

The objective of this project is to reduce manual Splunk configuration and provide a repeatable method for deploying Splunk components across development and production environments.

## Supported Splunk Components

The repository includes automation for:

- Cluster Manager
- Indexer Cluster Members
- Search Head Cluster Members
- Search Head Deployer
- Deployment Server
- Heavy Forwarder
- License Manager
- Monitoring Console

## Key Automation Areas

- Splunk installation
- Splunk service management
- Indexer cluster configuration
- Search Head cluster configuration
- Cluster Manager configuration
- Search Head Deployer configuration
- Deployment Server configuration
- Deployment client configuration
- Heavy Forwarder configuration
- License Manager connectivity
- Distributed search configuration
- Custom index creation
- Application deployment
- Indexer cluster bundle deployment
- Search Head cluster bundle deployment
- Splunk restart and status validation

## Repository Structure

```text
splunk-ansible-automation/
├── inventory/
│   └── dev/
│       ├── hosts.ini
│       └── group_vars/
│
├── playbooks/
│   ├── cluster-manager.yml
│   ├── indexer.yml
│   ├── search-head.yml
│   ├── deployer.yml
│   ├── deployment-server.yml
│   ├── heavy-forwarder.yml
│   ├── license-manager.yml
│   └── monitoring-console.yml
│
├── roles/
│   ├── cluster-manager/
│   ├── indexer/
│   ├── search-head/
│   ├── deployer/
│   ├── deployment-server/
│   ├── heavy-forwarder/
│   ├── license-manager/
│   └── monitoring-console/
│
├── ansible.cfg
└── README.md

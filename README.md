# Kubernetes Cluster Setup with Vagrant

This project provides a simplified way to set up a Kubernetes cluster using Vagrant. It automates the process of creating control plane (master) and worker nodes, installing necessary software components, and configuring Kubernetes.

## Prerequisites

Before you begin, ensure you have the following:

- VirtualBox
- Vagrant

## Getting Started

1. Clone this repository to your local machine:

   ```sh
   git clone https://github.com/Fahd-DevOps/Vagrant_K8s.git
   cd Vagrant_K8s
## Customize the cluster settings:

2. Modify the settings.yml file to specify the network configuration, node resources, and software versions.

Run the Vagrant environment:

   ```sh
   vagrant up
   ```
   - Wait for the provisioning to complete. The control plane (master) and worker nodes will be set up according to your configuration.
   
## Project Structure
  ```sh
     Vagrant_K8s/ 
    ├── scripts/
    │   ├── common.sh
    │   ├── master.sh
    │   └── node.sh
    ├── Vagrantfile
    └── settings.yml
  ```
  - scripts/: This directory contains provisioning scripts for control plane, worker nodes, and common setup.
  - Vagrantfile: Defines the configuration for your Vagrant environment.
  - settings.yml: Configuration file to customize cluster settings.
    
## Configuration
- Modify the settings.yml file to configure network settings, node resources, and software versions.

## Usage
- Run ``` vagrant up ``` to start the Kubernetes cluster.
- Use ``` vagrant ssh <node_name> ``` to access specific nodes via SSH.

## Cleanup
- When you're done using the cluster, you can clean up the environment:

```sh
vagrant destroy -f
```
$${\color{lightblue}Eng \space \color{lightgray}Fahd \space \color{lightgray}Khaled}$$

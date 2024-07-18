# Vagrant-Ansible-Ubuntu22.04-Minikube-Setup

This repository provides a fully automated setup for configuring Ubuntu 22.04 on one computer and Minikube on another using Vagrant and Ansible. This setup aims to streamline the development environment for containerized applications and Kubernetes-based projects.

## Introduction

This project automates the installation and configuration of two virtual machines:
- **Ubuntu 22.04**: A standard development environment.
- **Minikube**: A local Kubernetes cluster.

## Prerequisites

Before you begin, ensure you have the following installed:
- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) or another Vagrant provider
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/Vagrant-Ansible-Ubuntu22.04-Minikube-Setup.git
   cd Vagrant-Ansible-Ubuntu22.04-Minikube-Setup

2. **Initialize and start the Vagrant environment:**
    ```sh 
    vagrant up

3. **Usage**
- Access the Ubuntu 22.04 VM:
    ```sh 
    vagrant ssh ubuntu
-   Access the Minikube VM:
    ```sh 
    vagrant ssh minikube

You can now use these environments for your development and testing needs.
# README for Configuration Directory

This directory contains configuration files essential for the OpenShift airgap deployment project. It serves as a central location for managing various configuration settings that are crucial for the successful deployment and operation of the OpenShift cluster in an airgap environment.

## Overview

The configuration files in this directory are designed to be easily customizable to fit the specific needs of your deployment. Ensure that you review and modify these files as necessary before proceeding with the deployment process.

## Contents

- **install-config.yaml**: Contains the installation configuration for the OpenShift cluster.
- **agent-config.yaml**: Configuration for agents used in the deployment.
- **imageset-config.yaml**: Configuration for image sets used in the deployment.

For detailed instructions on how to use these configuration files, please refer to the respective documentation in the `docs/` directory.



```
ansible/
├── README.md
├── inventory.ini
├── group_vars/
│   └── all.yml
├── host_vars/
│   └── <hostname>.yml
├── playbooks/
│   ├── setup-mirror-registry-host.yml
│   ├── setup-oc-tools-host.yml
│   ├── setup-bootstrap-host.yml
│   ├── setup-oc-downloader-host.yml
│   └── site.yml                # Orchestrates all host setup playbooks
├── roles/
│   ├── create-vsphere-vm/
│   ├── configure-networking/
│   ├── install-openshift-tools/
│   ├── install-dnf-tools/
│   ├── install-foss-tools/
│   ├── configure-firewall/
│   ├── configure-storage/
│   └── ... (other modular roles as needed)
```
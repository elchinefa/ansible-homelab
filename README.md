# Setup Ubuntu Server for Kubernetes

This Ansible playbook is designed to automate the setup of Ubuntu Server for Kubernetes. It sets up hostnames, configures IP addresses and netplan, enables IP forwarding, removes machine IDs, configures sysctl settings, installs containerd, adds Kubernetes APT repository, installs required packages, and installs Kubernetes packages.

## Prerequisites

- Ansible installed on the control node
- Target hosts running Ubuntu Server

## Usage

1. Clone this repository:

    ```bash
    git clone https://github.com/elchinefa/ansible-homelab.git
    cd ansible-homelab
    ```

2. Modify the `hosts.yaml` file to match your environment. You can specify the IP addresses and second IPs for each host.

3. Execute the playbook using the following command:

    ```bash
    ansible-playbook -i hosts.yaml playbook.yaml
    ```

## Playbook Structure

- `playbook.yaml`: Main playbook file containing tasks for setting up Ubuntu Server for Kubernetes.
- `hosts.yaml`: Inventory file containing the IP addresses of the target hosts.


## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or create a pull request.


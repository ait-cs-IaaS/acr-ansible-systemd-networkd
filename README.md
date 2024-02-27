# Ansible-Role: acr-ansible-systemd-networkd

AIT-CyberRange: Manages the networkd service.


## Requirements

- Debian or Ubuntu 

## Role Variables

```yaml
networking_extra_configs: []

```

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - acr-ansible-systemd-networkd
      vars:
        networking_extra_configs: [{'network_conf': '10-netplan-ens4.network', 'domains': ['~austricom.at']}]
```

## License

GPL-3.0

## Author

- Lenhard Reuter
# Ansiblizing Proxmox

In the interest of repeatability, I upgraded a lot of my one-off home infrastructure by putting the provisioning behind [ansible](https://www.ansible.com) playbooks.

This wouldn't be possible without the excellent [ansible proxmox module](https://docs.ansible.com/ansible/latest/modules/proxmox_module.html).

This work establishes a few ansible roles
* [dist_upgraded](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/dist_upgraded) - Simple module to avoid having to have an `apt-get dist-upgrade` in every other role 
* [localized](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/localized) - Force a host to use a specific local file encoding
* [ntp](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/ntp) - Synchronize a host with NTP servers
* [open_jdk](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/open_jdk) - Installs OpenJDK on the host
* [proxmox_node](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/proxmox_node) - Provision a host to be a proxmox node
* [proxmox_lxc](https://github.com/LiquoriceLabs/ansible-public/tree/master/roles/proxmox_lxc) - Create and provision a proxmox container on a proxmode node

There are also a few samples for how to apply these roles.

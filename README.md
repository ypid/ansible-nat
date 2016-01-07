## [![DebOps project](http://debops.org/images/debops-small.png)](http://debops.org) nat

<!-- This file was generated by Ansigenome. Do not edit this file directly but
     instead have a look at the files in the ./meta/ directory. -->

[![Travis CI](http://img.shields.io/travis/debops/ansible-nat.svg?style=flat)](http://travis-ci.org/debops/ansible-nat) [![test-suite](http://img.shields.io/badge/test--suite-ansible--nat-blue.svg?style=flat)](https://github.com/debops/test-suite/tree/master/ansible-nat/)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-debops.nat-660198.svg?style=flat)](https://galaxy.ansible.com/detail#/role/1578)

### Warning, this is a deprecated role.

It has been superseded by [debops.subnetwork](https://github.com/debops/ansible-subnetwork).

***

`debops.nat` is a helper role which configures internal network on
a separate bridge interface with NAT or MASQUERADE firewall configuration
(the network will use a non-routable IP address space and access to the Internet
will be provided by the host operating system). This network can be used as
a development environment for virtual machines or containers.

Configuration of iptables firewall, forwarding and network interfaces will
be performed by the `debops.ferm` and `debops.ifupdown` roles.

You can use `dnsmasq` server (available via `debops.dnsmasq` Ansible
role) to complete the network configuration and provide internal DNS/DHCP
server.

### Installation

This role requires at least Ansible `v1.7.0`. To install it, run:

```Shell
ansible-galaxy install debops.nat
```

### Documentation

More information about `debops.nat` can be found in the
[official debops.nat documentation](http://docs.debops.org/en/latest/ansible/roles/debops.nat.html).


### Role dependencies

- `debops.ifupdown`
- `debops.ferm`

### Are you using this as a standalone role without DebOps?

You may need to include missing roles from the [DebOps common
playbook](https://github.com/debops/debops-playbooks/blob/master/playbooks/common.yml)
into your playbook.

[Try DebOps now](https://github.com/debops/debops) for a complete solution to run your Debian-based infrastructure.





### Authors and license

`nat` role was written by:

- Maciej Delmanowski | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)

License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

***

This role is part of the [DebOps](http://debops.org/) project. README generated by [ansigenome](https://github.com/nickjj/ansigenome/).

# VagrantLab

Vagrant based lab for quick testing of the new ideas on different Linux
distributions.

## Getting Started

These instructions will get you a copy of the project up and running on your
local machine for development and testing purposes. See deployment for notes on
how to deploy the project on a live system.

### Prerequisites

This lab require couple things to run. I made some assumptions here, and because
of that I won't describe whole installation of components required to run this
lab. Below I placed list of required software:

1. VirtualBox
2. Vagrant
3. Ansible
4. Git

If You want, You can adjust Vagrant file to use different hypevisior like i.e.
KVM or any other supported.

### Installing

Installation is simple as clone project from GitHub and then run command:

```
vagrant up
```

## Running the tests

Automated test hadn't been included to this project.

## Deployment

Deployment had been described in installing section.

## Built With

* [VirtualBox](https://www.virtualbox.org/) - Open-source hypervisor for x86 computers.

* [Vagrant](https://www.vagrantup.com/) -  Software for building and maintaining portable virtual software development environments.

* [Ansible](https://www.ansible.com/) - Software that automates software provisioning, configuration management,and application deployment.

* [kamikazestar.AnsibleRoleOsLinuxUpgrade](https://github.com/kamikazestar/AnsibleRoleOsLinuxUpgrade) - Role required to upgrade operating systems.

* [Git](https://github.io/) - Version control system.

## Versioning

I'm using standard GitHub workflow. For the versions available, see the [tags on this repository](https://github.com/kamikazestar/VagrantLab/tags).

## Authors

* **Marcin Slabonski** - *Initial work* - [kamikazestar](https://github.com/kamikazestar)

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/kamikazestar/VagrantLab/blob/master/LICENSE)
file for details.

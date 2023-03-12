# MY ANSIBLE FOR INSTALL STUFF ON NEW MACHINE

_TODO_:

- Make sure normal user in groups: _libvirt docker wheel phnaharris libvirtd_.
- Make script to run automatically.

## Installation

Make sure that you have **Ansible** installed on your machine.

To install Ansible, you can follow the Ansible Installation Guide at
[here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

### pip

```
python3 -m pip install --user ansible
```

### Arch Linux

```
sudo pacman -S ansible
```

### Ubuntu

_Debian have something different. Please refer to Ansible documentation to
install correctly._

```
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

### Fedora

```
sudo dnf install ansible
```

### CentOS

```
sudo yum install epel-release
sudo yum install ansible
```

After install Ansible, you can run the playbook with following command:

```
ansible-playbook localhost.yml --ask-become-pass
```

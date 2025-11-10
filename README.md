### For what?
Automatically install and configure 3proxy on Ubuntu 20+ to use proxy.
Proxy's kinda vpn.

### Configure app
Before installing the 3proxy, you have to have an installed ansible and obtained remote server.

Then configure 2 files:

1. 'ansible_host', 'ansible_user' and 'ansible_password' in the file:
`ansible-install-3proxy/inventory/hosts.yml`
2. 'vpn_login', 'vpn_password' and 'vpn_port' in the file:
`configure-3proxy/defaults/main.yml`

### Install 3proxy
In the root directory open the terminal and execute.
```cmd
ansible-playbook playbook/3proxy.yml
```

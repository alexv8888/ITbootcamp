## _Description_

This playbook adds users for the l2tp vpn to the Mikrotik router and creates passwords for them. Usernames are stored in the vault.yaml.

## _How to use_

- Set the router ip in the inv.yaml
- Put the vpn profile name and usernames in the vault.yaml
- Run: 
```sh
ansible-playbook -i inv.yaml routeros.yaml --ask-vault-pass
```
- Generated passwords are stored in /tmp/passwords/{{ username }}

Result example:

![winbox_window](winbox.jpg)

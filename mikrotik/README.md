## _Description_

This playbook adds users for the l2tp vpn to the Mikrotik router. Usernames ans passwords are stored in the vault.yaml.

## _How to use_

- Set the router ip in the inv.yaml
- Put vpn profile name, usernames and passwords of the users in the vault.yaml
- Run: 
```sh
ansible-playbook -i inv.yaml routerostest.yaml --ask-vault-pass
```
Result example:

![winbox_window](winbox.jpg)

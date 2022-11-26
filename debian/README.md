## _Description_

This playbook does the following:
- Disable root login over SSH
- Disable password login over SSH
- Add users and their public keys to the authorized_keys files

## _How to use_

- Set the server ip and the username in inv.yaml
- Put usernames and keys of the users to be created
- Run: 
```sh
ansible-playbook -i inv.yaml sslhardening.yaml --ask-become-pass --ask-vault-pass
```
### Ansible

To deploy

```bash
python3 -m pip install --user pipx
pipx install ansible
sss-add key.pem

ansible-playbook -i inventories/ccc_prod/ superset.yml --ask-vault-pass -e @inventories/ccc_prod/group_vars/superset/vars.yml -e @inventories/ccc_prod/group_vars/superset/vault.yml
```

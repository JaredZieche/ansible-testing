# Ansible Testing with vault
1. set `VAULT_ADDR` environment variable and log in to vault
```shell
export VAULT_ADDR='myvault_url'
vault login my_vault_login_method_or_cred
```
1. Run playbook
```
ansible-playbook -i inventory/inventory.yml playbook.yml -e "env=your_env"
```

# Install Ansible dependencies
```
ansible-galaxy install -r dependencies.yml -p vendor
```

# Provisioning
To provision a **development** machine:
```
ansible-playbook coopdevs.yml --ask-become-pass --limit=dev
```
To provision a **production** machine:
```
ansible-playbook coopdevs.yml --ask-become-pass --ask-vault-pass --limit=production
```

## How To Use ?
#### To Grant SSH ACCESS
```ansible-playbook -i inventory/ -e "action=grant" playbooks/ssh.yml```

#### To Revoke SSH Access
```ansible-playbook -i inventory/ -e "action=revoke" playbooks/ssh.yml --skip-tags=remove```

## Workflow
- Add IPs or DNS Name Under `servers` group in `inventory/hosts` files.
- Update the varibale "user_name" and "user_des" as per requirements. Y
- Make sure to create a directory under "sshkeys" directory of same name as user name and put its SSH pub key under it.

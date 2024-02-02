# Go Language installation via Ansible playbook

  * This installs the [Go Language](https://go.dev/) tools on Linux systems

## General information
  * In 'group_vars/all/vars.yml' you can specify the Go version you would like to download and install (See: [Go versions](https://go.dev/dl/))
  * Adjust the 'inventory' file to your needs.

### Run the Ansible playbook:
```zsh
ansible-playbook -i inventory main.yml
```

See: [Ansible documentation](https://docs.ansible.com/)

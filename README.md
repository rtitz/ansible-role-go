# Go Language installation via Ansible playbook

  * There is also an [Ansible Collection for Go](https://github.com/rtitz/ansible-collection-go) available, you can use that instead of this single role.
  * This installs the [Go Language](https://go.dev/) tools on Linux and macOS systems

## General information
  * In 'group_vars/all/vars.yml' you can specify the Go version you would like to download and install (See: [Go versions](https://go.dev/dl/))
  * Adjust the 'inventory' file to your needs.

### Run the Ansible playbook:
```zsh
ansible-playbook -i inventory main.yml -K 
```
  * Ansible will ask for the 'BECOME password', this is your sudo password
  * After the installation a reboot is needed, to ensure that the new environment variables are loaded correctly

See: [Ansible documentation](https://docs.ansible.com/)

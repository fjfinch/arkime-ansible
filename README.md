# arkime-ansible
COMING SOON

## Install & setup
To use this repo, a couple of tools are required:

* git (to clone the repo)
* pipx (to install ansible)
* ansible (to configure the system)

1 - Oneliner to install all above:
```bash
sudo apt update && sudo apt install -y git pipx && pipx install ansible --include-deps && pipx ensurepath && exec $SHELL
```

2 - Clone this repository:
```bash
git clone https://github.com/fjfinch/arkime-ansible.git
```

3 - Pull required roles:
```bash
ansible-galaxy collection install -r requirements.yml
```

4 - In `ansible/`, change the variables in `main.yml` & execute the playbook:
```bash
ansible-playbook main.yml -K
```

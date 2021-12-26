1. Enable the Ubuntu Universe repository:

   `sudo add-apt-repository universe`

2. Install Ansible:

   `sudo apt update`

   `sudo apt install software-properties-common`

   `sudo apt-add-repository --yes --update ppa:ansible/ansible`

   `sudo apt install ansible`

3. Clone repo:

   `git clone https://github.com/cch7e/ansible-vps.git && cd ansible-vps`

4. Change ip addr in `inventory`.

5. Change settings in `group_vars/all.yml`.

6. Run the playbook - something like `ansible-playbook -i inventory vps.yml -u root -k --ask-vault-pass` should do you nicely.


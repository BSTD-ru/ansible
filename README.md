Hosts `/etc/ansible/hosts`

    ansible --list-hosts all

Everyday commands:

    ansible-lint playbook.yml
    ansible-playbook --syntax-check playbook.yml
    ansible-playbook playbook.yml --extra-vars "target=1.1.1.1"

If there is `/etc/ansible/hosts` with a correct section in it:

    ansible-playbook playbook.yml
    ansible-playbook playbook.yml --limit=1.1.1.1

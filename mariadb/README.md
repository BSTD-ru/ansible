Set up master:

    ansible-playbook mariadb/master.yml --extra-vars "target=<..>"

Get master info on a master machine:

    SHOW MASTER STATUS;

Set up slave with master info:

    ansible-playbook mariadb/slave1.yml --extra-vars "target=<..> master=<..> master_port=<..> log_file=<..> log_pos=<..>"

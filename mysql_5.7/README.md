Set up master:

    ansible-playbook mysql_5.7/master.yml --extra-vars "target=<..>"

Get master info on a master machine:

    SHOW MASTER STATUS;

Set up slave with master info:

    ansible-playbook mysql_5.7/slave1.yml --extra-vars "target=<..> master=<..> master_port=<..> log_file=<..> log_pos=<..>"

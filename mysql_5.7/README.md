Set up master:

    ansible-playbook mysql_5.7/master.yml --extra-vars "target=<..>"

Get master info on master machine:

    SHOW MASTER STATUS;

Set up slave with master info:

    ansible-playbook mysql_5.7/slave1.yml --extra-vars "target=<..> master=<..> log_file=<..> log_pos=<..>"

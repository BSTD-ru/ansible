Get master info on master machine:

    SHOW MASTER STATUS;

Update slave with master info:

    ansible-playbook mysql_5.7/slave1.yml --extra-vars "target=<..> master=<..> log_file=<..> log_pos=<..>"

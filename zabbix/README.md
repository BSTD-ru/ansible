Zabbix agent example:

    ansible-playbook zabbix/agent.yml --extra-vars "target=<..> server=<..>"

Zabbix agent with MySQL support example:

    ansible-playbook zabbix/agent_mysql.yml --extra-vars "target=<..> server=<..>"

It is necessary to set Macro `{$MYSQL.DSN}` to `tcp://localhost:3306` or `unix:/var/run/mysqld/mysqld.sock`. And import and use new template `template_db_mysql_agent2.xml`.

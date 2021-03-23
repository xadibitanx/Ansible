## Ansible - Dynamic Inventory
- This includes ansible-playbook roles installation by Ansible - Dynamic Inventory plugin

- In order to make all this work follow this steps

1. use ansible above 2.9 version - you can find upgrade steps here https://stackoverflow.com/questions/34903026/update-ansible-1-9-4-to-ansible-2-0
2. use the lastes version of aws-cli
3. run pip3 install ansible
4. add in the right blocks ansible.cfg --- > /etc/ansible/ansible.cfg

[defaults]
inventory      = /home/ubuntu/ansible/aws_ec2.yml
host_key_checking = False


[inventory]
enable_plugins = aws_ec2, host_list




# ansible-playbook
This page explains how to run ansible playbook using dynamic inventory on the basis of autoscaling group and running the main playbook using that dynamic inventory and running that playbook using Jenkins job itself and sending job status on teams through teams web hook url on daily basis using jenkins periodic build
Jenkins node have outbound rules for ECS instances to connect.
- ECS instances have the necessary inbound rules for traffic to come through jenkins node.
- Python, Ansible and others dependencies like boto3, botocore should be installed. 
- Dynamic inventory plugin should be installed and make sure to enable it in the config file.
- Filter plugin should also be enabled and host_key_checking you can set it to false in config file and make user to ec2.
Reference-
https://docs.ansible.com/ansible/latest/collections/amazon/aws/aws_ec2_inventory.html

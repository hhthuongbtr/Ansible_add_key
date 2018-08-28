ansible-playbook -i hosts deploy/nginx.yml -u thuonghh -s
ansible-playbook -i hosts deploy/addKey.yml -u thuonghh -s
ansible -m shell -i hosts all -a uname -a -u thuonghh -s
ansible-playbook -i hosts deploy/nginx.yml -u thuonghh -s --list-host --list-task

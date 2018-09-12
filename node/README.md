# ansible-playbook
使用

先下载node放到/etc/ansible/roles/node/files/

mkdir -p /etc/ansible/roles/node/{defaults,files,tasks,templates,vars,handlers}

cd /etc/ansible/roles/node

ansible-playbook -i /etc/ansible/cloud.hosts node.yml -e 'hosts_group=cloud'

cat /etc/ansible/cloud.hosts

```
[cloud]
cloud-6 ansible_ssh_host=192.168.20.227 ansible_ssh_user=root
```


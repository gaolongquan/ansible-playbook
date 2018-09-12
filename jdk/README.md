# ansible-playbook
使用

先下载jdk放到/etc/ansible/roles/jdk/files/

mkdir -p /etc/ansible/roles/jdk/{defaults,files,tasks,templates,vars,handlers}

cd /etc/ansible/roles/jdk

ansible-playbook -i /etc/ansible/cloud.hosts jdk.yml -e 'hosts_group=cloud'

cat /etc/ansible/cloud.hosts

```
[cloud]
cloud-6 ansible_ssh_host=192.168.20.227 ansible_ssh_user=root
```


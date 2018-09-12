# ansible-playbook
使用

先下载apache-maven放到/etc/ansible/roles/apache-maven/files/

mkdir -p /etc/ansible/roles/apache-maven/{defaults,files,tasks,templates,vars,handlers}

cd /etc/ansible/roles/apache-maven

ansible-playbook -i /etc/ansible/cloud.hosts apache-maven.yml -e 'hosts_group=cloud'

cat /etc/ansible/cloud.hosts

```
[cloud]
cloud-6 ansible_ssh_host=192.168.20.227 ansible_ssh_user=root
```


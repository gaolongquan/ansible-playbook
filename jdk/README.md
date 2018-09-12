# ansible-playbook
使用

cd /etc/ansible/roles/jdk

mkdir -p {defaults,files,tasks,templates,vars,handlers}

ansible-playbook -i /etc/ansible/cloud.hosts jdk.yml -e 'hosts_group=cloud'

cat /etc/ansible/cloud.hosts

[cloud]
cloud-6 ansible_ssh_host=192.168.20.227 ansible_ssh_user=root

 ll /etc/ansible/roles/jdk/files/
-rw-r--r-- 1 root root 190890122 Sep 12 12:36 jdk-8u171-linux-x64.tar.gz

# ha-kubernetes-kubeadm
Ansible Playbooks to install an HA Kubernetes
- Install Ansible: 
`yum install ansible`
- Setup ssh access from Ansible host to Kubernetes nodes.
```ssh-copy-id -i ~/.ssh/id_rsa.pub <user@host>```
You can now run install-all.yaml playbook to get your cluster setup.
```
ansible-playbook -i inventory/cluster1-prod playbooks/install-all.yaml --private-key=~/.ssh/id_rsa -u %username% -v
```

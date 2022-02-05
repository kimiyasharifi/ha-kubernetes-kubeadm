# ha-kubernetes-kubeadm
Ansible Playbooks to install an HA Kubernetes
# Prerequisites:
- Install Ansible: 
`yum install ansible`
- Setup ssh access from Ansible host to Kubernetes nodes.
```ssh-copy-id -i ~/.ssh/id_rsa.pub <user@host>```

# Install a highly available kubernetes using kubeadm
```
ansible-playbook -i inventory/cluster1-prod playbooks/install-all.yaml --private-key=~/.ssh/id_rsa -u %username% -v
```

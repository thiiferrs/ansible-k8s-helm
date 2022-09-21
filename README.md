## Ansible k8s Helm install stack

---

included tasks tools: cluster-autoscaler, metrics-server, prometheus, kube-state-metrics, traefik

### Requeriments:

* EKS cluster
* Python 3.5+
* Ansible 2.9
* Helm v3.7+
* [Kubernetes Collection for Ansible](https://galaxy.ansible.com/kubernetes/core?extIdCarryOver=true&sc_cid=701f2000001OH7YAAW)

Kubernetes Collection for Ansible module documentation: https://docs.ansible.com/ansible/latest/collections/kubernetes/core/index.html

### Use

1. Configure AWS Cli or Secrets
2. Define group_vars/all.yaml
3. Run:
```
$ ansible-playbook site.yaml -i hosts -t all
```

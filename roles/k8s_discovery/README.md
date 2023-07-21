k8s_discovery
=========

Tooling to support the dynamic discovery of VirtualMachine instances and facilitating their assignment into an Ansible
inventory

Role Variables
--------------

| Variable            | Description            | Default |
|:--------------------|:-----------------------|:--------|
| `k8s_group_label`   | `group level of k8s`   | ` `     |
| `k8s_resource_type` | `resource type of k8s` | `pods`  |

Dependencies
------------

* [kubernetes.core](https://docs.ansible.com/ansible/latest/collections/kubernetes/core/index.html)
* [ansible.controller](https://docs.ansible.com/automation.html)
* [redhat_cop.controller_configuration](https://galaxy.ansible.com/redhat_cop)

Example Playbook
----------------

Please follow [k8s_discovery.yml](https://github.com/ansible-middleware/ocpv_lab/blob/main/playbooks/k8s_discovery.yaml)
for better understanding.

License
-------

[Apache License Version 2.0](https://github.com/ansible-middleware/ocpv_lab/blob/main/LICENSE)


Author Information
------------------

- [Andrew Block](https://github.com/sabre1041)
- [Guido Grazioli](https://github.com/guidograzioli)
- [Ranabir Chakraborty](https://github.com/RanabirChakraborty)

configure_aap
=========

Configurations to prepare Ansible Automation Platform for use managing the assets related to the Ansible Middleware
OpenShift Virtualization Lab.

Role Variables
--------------

| Variable                                         | Description                                  | Default                                                                            |
|:-------------------------------------------------|:---------------------------------------------|:-----------------------------------------------------------------------------------|
| `aap_controller_namespace`                       | `namespace of AAP controller`                | `ansible-automation-platform`                                                      |
| `aap_openshift_serviceaccount_name`              | `name of AAP openshift serviceaccount`       | `aap-ocpv`                                                                         |
| `aap_openshift_serviceaccount_token_name`        | `token name of AAP openshift serviceaccount` | `"{{  aap_openshift_serviceaccount_name}}-token"`                                  |
| `aap_credential_type_redhat_serviceaccount_name` | `Red Hat AAP service account name`           | `Red Hat Service Account`                                                          |
| `aap_credential_type_publickey_name`             | `AAP publick key credential type`            | `SSH Public Key`                                                                   |
| `aap_credential_type_redhat_csp_name`            | `CSP name crdential type`                    | `Red Hat Customer Portal`                                                          |
| `aap_credential_machine_name`                    | `machine name which is using AAP credential` | `OCPv SSH`                                                                         |
| `aap_credential_jbossnetwork_name`               | `JBoss network name credential type`         | `JBossnetwork API`                                                                 |
| `aap_credential_openshift_name`                  | `Openshift name credential type`             | `OCP`                                                                              |
| `aap_credential_redhat_csp_name`                 | `Red Hat CSP name credential type`           | `RHN`                                                                              |
| `aap_credential_openshift_host`                  | `Openshift host link`                        | `https://kubernetes.default.svc`                                                   |
| `aap_credential_publickey_name`                  | `provided name of public key`                | `OCPv Public Key`                                                                  |
| `aap_credential_automationhub_name`              | `Automation Hub name`                        | `Automation Hub`                                                                   |
| `aap_inventory_ocpv_name`                        | `OCPV name`                                  | `ocpv`                                                                             |
| `aap_inventory_ocpv_eap_name`                    | `OCPV EAP name`                              | `eap`                                                                              |
| `aap_template_deploy_ocp_playbook`               | `path of OCPV install playbook`              | `playbooks/install_ocpv.yml`                                                       |
| `aap_template_deploy_lab_playbook`               | `path of lab deploy playbook`                | `playbooks/deploy_lab.yml`                                                         |
| `aap_project_ocpv_name`                          | `OCPV lab name`                              | `ocpv_lab`                                                                         |
| `aap_project_ocpv_git_url`                       | `OCPV dmeo GitHub url`                       | `https://github.com/ansible-middleware/ocpv_lab.git`                               |
| `aap_project_ocpv_git_branch`                    | `OCPV lab branch name`                       | `main`                                                                             |
| `automationhub_server_url`                       | `Automation Hub server URL`                  | `https://cloud.redhat.com/api/automation-hub/ `                                    |
| `automationhub_auth_server_url`                  | `Automation Hub authentication server url`   | `https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token` |
| `ocpv_ssh_user`                                  | `OCPV ssh username`                          | `cloud-user`                                                                       |
| `aap_organization`                               | `AAP organization name`                      | `Default`                                                                          |
| `lab_namespace`                                  | `OCPV lab namespace`                         | `ansible-middleware-ocpv`                                                          |
| `lab_name`                                       | `deployed lab name`                          | `eap-lab`                                                                          |

Dependencies
------------

* [kubernetes.core](https://docs.ansible.com/ansible/latest/collections/kubernetes/core/index.html)
* [ansible.controller](https://docs.ansible.com/automation.html)
* [infra.controller_configuration](https://galaxy.ansible.com/infra)

Example Playbook
----------------

License
-------

[Apache License Version 2.0](https://github.com/ansible-middleware/ocpv_lab/blob/main/LICENSE)

Author Information
------------------

- [Andrew Block](https://github.com/sabre1041)
- [Guido Grazioli](https://github.com/guidograzioli)
- [Ranabir Chakraborty](https://github.com/RanabirChakraborty)

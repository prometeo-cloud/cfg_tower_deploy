### cfg_tower_deploy

## Description:

- cfg_tower_deploy runs a playbook which uses the tower_install_application role to automate the provisioning of an Ansible Tower instance. </br>
- cfg_tower_deploy runs a playbook which uses the configure_ansible_tower role to automate the configuration setting of an Ansible Tower instance.</br>

## Behaviour:

Feature:</br>
- Runs tower_install_application role. As a System Admin I want to install automate the installation of Tower, which can be configured for use by my organisation.
- Runs tower_configure_application role. As a System Admin I want to automate the configuration and running of Tower workflows for my organisation.</br>

## Dependencies:

- tower_install_application role</br>
- tower_configure_application role</br>
- Preconfigured RHEL 7.x machine</br>

## Testing the role:
```---
# - hosts: towers
  name: Install and configures a tower based upon requirements gathered. 
  roles:
    - install_ansible_tower
    - tower_configure_application
```


# drone-plugin-ansible-lint
Drone plugin to provision infrastructure with Ansible.

## Example pipeline
```
kind: pipeline
name: default

steps:
- name: Lint ansible playbook
  image: getais/drone-plugin-ansible-lint
  commands:
    - ansible-lint some-playbook
```

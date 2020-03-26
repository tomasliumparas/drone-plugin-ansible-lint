
# drone-plugin-ansible-lint
Drone plugin to provision infrastructure with Ansible. Built form original plugin, packing ansible-lint

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

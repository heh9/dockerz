# Docker image with Ansible 2.4.2 installed

## Useful in automation scripts like Gitlab's CI.
```yaml
provision:
  stage: "provision"
  image: vladimiriacob/ansible-ci
  script:
    - ansible-playbook -i openstack.py site-playbooks/app.yml
  tags:
```

### Installed libs ( can also target windows machines )
#### ansible==2.4.2 shade==1.17.0 pywinrm==0.3.0 hvac==0.2.17

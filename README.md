# lab_my_ansible_project

My ansible project

## Best Practices

* Tree

https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html

## Test my project


* Test ansible.cfg

```
ansible localhost -m uri -a 'url=http://www.google.com/ return_content=yes'
```

* Test inventory file ./inventory_test

``` shell
ansible all -i inventory_test --list-hosts 
ansible db --list-hosts -i inventory_test
```

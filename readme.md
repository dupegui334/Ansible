1. PING:
- Give permissions to the key & run the commands:
```
    sudo chmod 600 key.pem
    sudo ansible all --key-file ./medina.pem -i inventory -m ping
```
2. First-paybook: First check the info of your servers with:
```
    sudo ansible all --key-file ./medina.pem -i ./inventory -m gather_facts

```
    - Then we install httpd or apache2 to the ec2 depending on the distro
```
    sudo ansible-playbook --key-file ./medina.pem -i inventory --ask-become-pass install_httpd.yml
```
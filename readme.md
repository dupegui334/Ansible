1. PING:
- Give permissions to the key & run the commands:
```
    sudo chmod 600 key.pem
    sudo ansible all --key-file ./medina.pem -i inventory -m ping
```
2. First-paybook: Here we install httpd to an Amazon Linux 2 ec2 or apache in Ubuntu
```
    sudo ansible-playbook --key-file ./medina.pem -i inventory --ask-become-pass install_httpd.yml
```


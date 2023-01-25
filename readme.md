1. PING:
- Give permissions to the key & run the commands:
```
    sudo chmod 600 key.pem
    sudo ansible all --key-file ./medina.pem -i inventory -m ping
```



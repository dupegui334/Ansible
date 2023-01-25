- Give permissions to the key:
    sudo chmod 600 key.pem

- Run the command:
    sudo ansible all --key-file ./medina.pem -i inventory -m ping
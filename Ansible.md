## run ansible ad-hoc command on vagrant maschine
`ansible -i 'localhost,' -u core --ssh-extra-args='-p 2200' --sftp-extra-args='-P 2200' --private-key=keys/coreos -m raw -a 'stat $HOME/.bootstrapped' localhost`


```shell
ssh_config=$(tempfile)
vagrant ssh-config node-3 > $ssh_config
ansible -i 'node-3,' --ssh-common-args="-F $ssh_config" -m raw -a 'stat $HOME/.bootstrapped' node-3
```

## run ansible ad-hoc command on vagrant maschine
`ansible -i 'localhost,' -u core --ssh-extra-args='-p 2200' --sftp-extra-args='-P 2200' --private-key=keys/coreos -m raw -a 'stat $HOME/.bootstrapped' localhost`


```shell
ssh_config=$(tempfile)
vagrant ssh-config node-3 > $ssh_config
ansible -i 'node-3,' --ssh-common-args="-F $ssh_config" -m raw -a 'stat $HOME/.bootstrapped' node-3
```

## IP-Adressen und Netz Funktionen in Ansible

https://docs.ansible.com/ansible/playbooks_filters_ipaddr.html

Benötigtes Packet: `pip install netaddr`

```python
kube_service_addresses: 172.28.128.0/24
skydns_server: "{{ kube_service_addresses|ipaddr('net')|ipaddr(3)|ipaddr('address') }}"
```

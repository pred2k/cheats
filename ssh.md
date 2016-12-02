
# SSH cheat codes

## key generation

```bash
ssh-keygen -t rsa -b 4096 -C "your@mailadress"
```

## list keysize and fingerprint:

```bash
    ssh-keygen -f $HOME/.ssh/id_rsa -l
```

## show fingerprint of known hosts
    ssh-keygen -l -F <HOSTNAME>

## remove key from known_hosts on server key change (-R hostname Remove host from known_hosts file.) (useful for hashed known_hosts)

    ssh-keygen -R hostname

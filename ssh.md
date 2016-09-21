
# SSH cheat codes

## key generation

```bash
ssh-keygen -t rsa -b 4096 -C "your@mailadress"
```

## list keysize and fingerprint:

```bash
    ssh-keygen -f $HOME/.ssh/id_rsa -l
```

## remove key from known_hosts on server key change (-R hostname Remove host from known_hosts file.)
    ssh-keygen -R hostname

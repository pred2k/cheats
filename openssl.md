
# Openssl Cheats


#### CSR anzeigen

    openssl req -text -noout -in <FILE>

#### TLS Verbindung aufbauen
    openssl s_client -showcerts -connect www.heise.de:443

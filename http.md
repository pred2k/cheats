
## [httpie](https://httpie.org) commands

### outout reponse header only

    http -h www.google.de

### Set Headers

    http example.org  User-Agent:Bacon/1.0  'Cookie:valued-visitor=yes;foo=bar'  X-Foo:Bar  Referer:http://httpie.org/

### Show request- and response-header and response body

    http -p Hhb httpbin.org/headers User-Agent:HTTPie Host:www.myhttptest.com

## curl commands

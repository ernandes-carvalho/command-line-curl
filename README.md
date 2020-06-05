# command-line-curl

Tutorial
 - Commands to use curl from the windows prompt

cURL [documentation](https://curl.haxx.se/docs/httpscripting.html)

### Exemples
Version
```sh
$ curl  -version
```
>curl --version
>curl 7.55.1 (Windows) libcurl/7.55.1 WinSSL
>Release-Date: [unreleased]
>Protocols: dict file ftp ftps http https imap imaps pop3 pop3s smtp smtps telnet tftp
>Features: AsynchDNS IPv6 Largefile SSPI Kerberos SPNEGO NTLM SSL

Download files
```sh
$ curl  -C - -O http://localhost/sql-database.bkp
```
> ** Resuming transfer from byte position 4991
>  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
>                                 Dload  Upload   Total   Spent    Left  Speed
>  0  4991    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0

POST
```sh
$ curl http://localhost/login.php --request POST --data "login=my-login&password=my-password"
```

GET
```sh
$ curl http://localhost/login.php
```

UPLOAD FILE
```sh
curl -F file=@backup.php http://localhost/uploads.php
```
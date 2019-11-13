# readme

1. gen key copy to Certificates
```
openssl req -newkey rsa:2048 -nodes -keyout my.key -x509 -days 365 -out my.cer
openssl pkcs12 -export -in my.cer -inkey my.key -out my.pfx
```

2. set my.pfx as Embedded resource

3. UseKestrel
# Spring Boot Json Web Token Using Asymmetric Key
We are going to implement JWT in spring boot application using RSA Public Private Key.

Command for creating RSA Public and Private Keys
```
openssl genrsa -out keypair.pem 2048

# Extract Public Key
openssl rsa -in keypair.pem -pubout -out public.pem

# create private key in PKCS#8 format
openssl pkcs8 -topk8 -inform PEM -outform PEM -nocrypt -in keypair.pem -out private.pem


```

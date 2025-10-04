---
title: "openssl"
draft: false
---

# openssl

## Issue all certificates in a chain

```bash
openssl s_client -showcerts -verify 5 -connect <host name>:443 -servername <host name>
```
 
```bash
openssl s_client -connect <hostname:port>
```

```bash 
openssl s_client -connect <hostname:port> -servername <hostname/url> | 
openssl x509 -text
```

## Convert DER to PEM

```bash
openssl x509 -inform der -in CERTIFICATE.der -out CERTIFICATE.pem
```

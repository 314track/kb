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
openssl x509 -inform der -in certificate.der -out certificate.pem
```

## Convert CER (binary) to PEM

```bash
openssl x509 -in certificate.crt -out certificate.pem -outform PEM
```

## Preparing certificate for haproxy

Starting with the server certificate, becoming more and more general (intermediate certificates, without the root ca), ending with the private key.

```bash
cat <certificate>.decer.cer ECC_D-TRUST_BR_CA_1-20-1_2020.cer ECC_D-TRUST_BR_Root_CA_1_2020.cer <private key>.key > output.pem
```

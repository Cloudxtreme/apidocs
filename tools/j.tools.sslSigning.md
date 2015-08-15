## j.tools.sslSigning

- /opt/jumpscale7/lib/JumpScale/baselib/sslsigning/SSLSigning.py

#### bundle 
- arguments
    - certificate
    - key
    - certification_chain = ()
    - passphrase
- comments
    Bundles a certificate with it's private key (if any) and it's chain of trust.
    Optionally secures it with a passphrase.

#### createCertificateSigningRequest 
- arguments
    - common_name
- comments
    

#### createSignedCert 
- arguments
    - path
    - keyname
- comments
    Signing X509 certificate using CA
    The following code sample shows how to sign an X509 certificate using a CA:

#### create_self_signed_ca_cert 
- arguments
    - cert_dir
- comments
    is for CA
    If datacard.crt and datacard.key don't exist in cert_dir, create a new
    self-signed cert and keypair and write them into that directory.

#### signRequest 
- arguments
    - req
    - ca_cert
    - ca_key
- comments
    


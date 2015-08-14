## j.tools.sslSigning

- /opt/jumpscale7/lib/JumpScale/baselib/sslsigning/SSLSigning.py

### def signRequest(req, ca_cert, ca_key) (l109)

### def createCertificateSigningRequest(common_name) (l92)

### def createSignedCert(path, keyname) (l64)

Signing X509 certificate using CA
The following code sample shows how to sign an X509 certificate using a CA:

### def bundle(certificate, key, certification_chain=(), passphrase=None) (l141)

Bundles a certificate with it's private key (if any) and it's chain of trust.
Optionally secures it with a passphrase.

### def create__signed_ca_cert(cert_dir) (l13)

is for CA
If datacard.crt and datacard.key don't exist in cert_dir, create a new
self-signed cert and keypair and write them into that directory.


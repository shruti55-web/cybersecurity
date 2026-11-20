Symmetric vs Asymmetric Encryption
Symmetric	                                                Asymmetric
Uses one shared secret key	                       Uses a public/private key pair
Fast for large amounts of data	                   Useful for key establishment and digital signatures
Example: AES	                                   Examples: RSA, elliptic-curve cryptography

Hashing — MD5 and SHA-256

- Hashing converts data into a fixed-length digest.
- MD5 produces a 128-bit digest but is insecure against collisions.
- SHA-256 produces a 256-bit digest and is widely used for integrity checks.
- Hashing is not the same as encryption; a hash is not designed to be decrypted.
- Passwords should be stored using dedicated password-hashing algorithms such as Argon2id, scrypt, or bcrypt.

Digital Certificates and SSL/TLS
- A digital certificate binds an identity, such as a domain name, to a public key.
- A Certificate Authority (CA) issues and digitally signs certificates.
- SSL is obsolete; TLS is its modern replacement.
- HTTPS uses TLS to provide confidentiality, integrity, and server authentication.
- Browsers check certificate validity, hostname, and trust chain.
- A valid certificate does not guarantee that a website is legitimate or free from vulnerabilities.
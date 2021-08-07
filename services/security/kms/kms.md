# Key Management Service (KMS)

Service to manage all your encryption keys and encryption.

## Customer Master Keys (CMK)

Two types:

### Symmetric (AES-256 keys)

Single key to encrypt and decrypt data.

### Asymmetric (RSA & ECC key pairs)

Two keys. Public key (encrypt) and private key (Decrypt). Used for sign and verify operations. e.g. TLS, SSL. e.g. encryption outside AWS.

*Note: Encrypted secrets can be stored in code / environment variables.*

## Automatic Key Rotation

Automatically change underlying encyption keys every x days. Only applicable for Customer Managed CMK.

## Access

Key Policy == IAM Policy
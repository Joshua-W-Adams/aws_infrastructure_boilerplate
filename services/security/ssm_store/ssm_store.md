# Systems Manager (SSM) Parameter Store

Service to store all your application parameters securely. e.g. user names and passwords for dbs.

i.e. just a store of the encrypted values.

Encryption is managed in KMS.

## Parameter Policies

Polciies can be assigned to parameters to enforce the following:

- TTLs (expiration)
- Notifications (alerts when keys havent been changed for x days)
- etc.

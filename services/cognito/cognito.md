# Cognito

Service for managing user authentication.

## Cognito User Pools (CUP)

AWS identity provider and user management service. Best explained by the diagram below.

![](./../../img/cognito_architecture.png)

Authorisation of users via:
- username, password, MFA
- Facebook, Google etc.

Supports:
- verification of emails and phone numbers

Returns a JSON Web Token (JWT) with authentication credentials.

## Identity Pools (Federated Identity)

Provide direct access to AWS Resources.

![](./../../img/federated_identity_pool.png)

## Cognito Sync

Stores preferences, configuration and state of application.

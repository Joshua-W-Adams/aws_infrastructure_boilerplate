# Network 

Uses security groups to manage access.

# User Management

User access is generally managed at the database level.

Notes:
- IAM policies only control who can create and manage the RDS

## IAM

IAM can be used to managed user access for MySQL, PostGres and Aurora DB engines as per the following diagram:

![](./../../../img/rds_iam_user_management.png)

## Encryption

Encryption can only be enabled when the database is first started.

You cannot enable encryption on an already running database.
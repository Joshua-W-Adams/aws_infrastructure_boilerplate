# Access

Access by users and services is governed by AWS IAM.

Access to buckets can be defined the following options:
- Bucket IAM Policies
- Access Control Lists (ACLs)
    - Obect and Bucket levels
- Presigned URLs - URL that is valid for a specific period of time and includes authentication info

*Note: Bucket Policies can be created that force encryption requirements by specifying the "conditions" property under the policy statement.*

## Encryption

### SSE-S3

Server Side Encryption (SSE) operations can be handled by S3.

- *AES-256 encryption alogrithm as standard*
- *HTTP header "x-amz-server-side-encryption": "AES256" specified with file upload to perform encryption.*

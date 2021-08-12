# Lambda

Virtual functions that run on demand.

- Scaling is automated.
- supports basically any language and even containers!!
- Extremely cheap
- Has a whole bunch of blueprints for common operations...

## Limits

Effectively you can run anything you want as the limitations are very generous.

- Memory: 128MB - 10GB
- Max Execution time: 900 seconds
- Environment variables: 4KB
- Disk Capacity: 512MB
- **Concurrency: 1000** - you can raise this by contacting AWS support
- Compressed deployment size: 50MB
- Uncompressed "": 250MB

## Languages Supported

- JavaScript
- Java
- C#
- Go
- Python
- Ruby

## Lambda at Edge

Deploy lambda functions at clound front locations.

Note: can modify request / responses on send and recieve totaling 4 events.

## Lambda VPC

By default, Lambda functions always operate from an AWS-owned VPC and hence have access to any public internet address or public AWS APIs.

Once a Lambda function is VPC-enabled, it will need a route through a NAT gateway in a public subnet to access public resources.

## Lambda Layers

packaged up re-useable code that can be used accross lambda functions.

Layers can be thought of as the domain layer code and lambda functions as the use cases.
# Auto Scaling Group (ASG)

Automatically scales ec2 instances up and down based on application load.

Simply group of ec2 instances and scaling configuration

Cnfiguration files include:

- VM configuration
    - AMI + Bootstrapping
    - EC2 type
    - EBS Volumes
    - Security Groups
- min / max sizes
- etc.

## Scaling Policies

Rules by which ASG are scaled in and out.

*Note: Cloud Watch can watch your ASG and scale it automatically for you.*

### Dynamic Scaling Policies

3 different types

Target
- a specific metric value e.g. 40% cpu
Step
- specificy ranges/steps to scale by. e.g. at 70% add 2 units, at 30% remove 1 unit
Scheduled
- add/remove units based on specific time frames

### Predictive Scaling

Continuously forecast load with machine learning and schedule scaling ahead of time.

### Metrics

The following are good metrics to scale by in your policies.

- CPU
- Network
    - Request count per target
    - Average traffic in and out

You can also scale by any other custom metrics you want.

## Cooldown Period

Duration between each scaling operation.

## Termination Policy

By default ASG will.

- Terminate the oldest EC2 running.
- Will try to balance across AZs.

## Lifecycle Hooks

You have the ability to perform additional steps before a new instance is put into or taken out of service.
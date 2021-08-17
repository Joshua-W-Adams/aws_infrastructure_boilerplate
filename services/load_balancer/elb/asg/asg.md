# Auto Scaling Group (ASG)

Automatically scales ec2 instances up and down based on application load.

Simply group of ec2 instances and scaling configuration

## Launch Configuration Files

ASGs can be created using a launch configuration file which contains the following information.

- VM configuration
    - AMI + Bootstrapping
    - EC2 type
    - EBS Volumes
    - Security Groups
- min / max sizes
- etc.

Launch configuration files are for 1 VM configuration only. Cannot be edited.

## Launch Templates

Newer version of launch configurations and adds the following additional features:

- Multiple versions
- combination of instance types
- combination of placement types (e.g. spot and on demand)

## Scaling Policies

Rules by which ASG are scaled in and out.

*Note: Cloud Watch can watch your ASG and scale it automatically for you.*

### Dynamic Scaling Policies

3 different types

Target
- a specific metric value e.g. 40% cpu
Simple
- define a single threshold value and specify scaling value. i.e @ 80% cpu add 20% capacity. @ 30% cpu remove 20% capacity.
Step
- An improved version of simple scaling whereby you specificy ranges/steps to scale by while an alarm is in progress. Allows adding of additional capacity without having to wait for the cooldown period to expire in a simple scaling policy. e.g. at 70% over threshold value add 2 units, at 30% over add 1 unit.
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
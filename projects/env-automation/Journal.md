## Journaling

## VPC Settings

These are the VPC Setiings I observed Tim setup 
for our cloud environment in AWS:

- VPC IPv4 CIDR Block: 10.200.123.0/24
- IPv6 CIDR Block: No
- Number of AZs: 1
- Number of public subnets: 1
- Number of private subnets: 1
- NAT Gateways: None
- VPC Endoints: None
- DNS Options: Enable DNS Hostnames
- DNS Options: Enable DNS Resolution

## Generated and Review CFN Template

Watching the isntructor videos, I noted the VPC settings, provided this to ChatGPT to produce the CFN template to automate the provision of the VPC infrastructure.

I had to ask the LLM to refactor the template parameters so that it would not hardcode the values and template is more usable.

## Generated Deploy Script

Using ChatGPT, generated a bash script `bin/deploy`

I changed the shebang to work for all OS platforms.

## Visualization in Infrastructure Composer

I thought may be we could visualize our VPC via infrastructure Composer but its not the best respresentation

![](/projects/env-automation/assets/aws_infr_composer.PNG)

## Installing AWS CLI

In order to deploy via AWS CLI, we need to install it.

I followed the instructions:
[AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

## Deployed Resource to AWS

This is the resource map of the VPC deployed with CFN.
![](/projects/env-automation/assets/aws_vpc_resource_map.PNG)


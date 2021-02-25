

## Cloudformation 101

#### Parameters

[Cloudformation Parameters](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/parameters-section-structure.html)


#### Resources

[Cloudformation Resources](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html)

#### Different types of resources and how they fit together

ie EC2 and its properties, Subnet, SG, AMI ID


#### Outputs


#### What are parameters and how we can feed them to a deployment to different enviroments and manage consistnent naming scheme

[Cloudformation Outputs](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/outputs-section-structure.html
)


### Objectives

##### - Manually create a KeyFile, to use with connecting to Instance

#####  - Create a Cloudformation Parameter (3389, Ports for SG) and use the !Sub Function to Import the value and to fill out a discription.

#####  - Create a Cloudformation Resource, (Security Group) and attach to a EC2 instance

##### - Create a Cloudformation Output (Public IP address for RDP)



## Cloudformation 201

#### Bootstrap Repo

### What is the Bootstrap repo and what is each module and how do they work

[Bootstrap Repo](https://github.com/MYOB-Technology/template-bootstrap-dx)


#### How to Clone/Fork Repo to start setting up a new account
    
#### Consuming outputs from different Stacks


#### Subs and other useful Functions

#### Style Guide

## Git/Github

#### Managing Branches and Deployment Stratergy

#### Creating Feature Branches
#### Pull Requests and Approvals and Merges
#### Deploying off Master or Release branch


## Buildkite

#### Creating a pipline with `pipe`

[Create a buildkite pipeline using MYOB's pipeline tool](https://github.com/MYOB-Technology/pipe))

#### Managing a Pipeline Deployment (Blocks, Branches)

[Buidkite Branching Strategy](https://buildkite.com/docs/pipelines/branch-configuration)

#### Pipeline Deploy Files (Docker, Makefile, Auth/Queues, Troubleshooting)


#### Docker
How Docker works and the make up of the Docker Compose File


[Makefile]

How we use the Makefile to standardise a deployment

[myob-auth]

How we auththenticate to a AWS account using myob-auth



## AWS

#### Best Practice Approach, Account Setup (SSVC vs Spoke)


#### Basics AWS Services, EC2, ELB, S3, VPC (Subnets, SGs, NACLs)


## Running Your Command

aws cloudformation deploy --template template.yml --stack-name samtest --parameter-overrides Name=Sam
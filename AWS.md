# AWS Naming Convention
Reference: [Cloud Conformity](https://www.trendmicro.com/cloudoneconformity-staging/knowledge-base/aws/)

&nbsp;
&nbsp;

## VPC Naming Conventions
### Default Pattern Format
`vpc-RegionCode-EnvironmentCode-ApplicationStackCode`

### Default Pattern Components
**Region Code**  
`(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)` etc.  

**EnvironmentCode**  
`(dev|test|stg|prod)` for development, test, staging, production.  

**ApplicationStackCode**  
`([a-z0-9\-]+)` for the application stack that runs within the VPC network.  

### RegExp
`^vpc-(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)-(dev|test|stg|prod)-([a-z0-9\-]+)$`

### Default Pattern Examples
`vpc-ap-northeast-1-prod-web-app-stack`  
`vpc-ap-northeast-2-dev-big-data-stack`  

&nbsp;
&nbsp;

## Subnet Naming Conventions
### Default Pattern Format
`subnet-RegionCode-AvailabilityZoneCode-SubnetRouteCode-EnvironmentCode-ApplicationStackCode`

### Default Pattern Components
**Region Code**  
`(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)` etc.  

**AvailabilityZoneCode**  
`([1-2]{1})([a-c]{1})`

**SubnetRouteCode**  
`(public|private)` for public and private subnet.

**EnvironmentCode**  
`(dev|test|stg|prod|mgmt)` for development, test, staging, production, management.  

**ApplicationStackCode**  
`([a-z0-9\-]+)` for the application stack that runs within the VPC network. 

### RegExp
`^subnet-(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)-([1-2]{1})([a-c]{1})-(public|private)-(dev|test|stg|prod|mgmt)-([a-z0-9\-]+)$`

### Default Pattern Examples
`subnet-ap-northeast-1-1a-public-prod-web-app-stack`  
`subnet-ap-northeast-1-1c-private-dev-database-stack`  

&nbsp;
&nbsp;

## Security Group Naming Conventions
### Default Pattern Format
`security-group-RegionCode-EnvironmentCode-ApplicationCode`

### Default Pattern Components
**Region Code**  
`(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)` etc.  

**EnvironmentCode**  
`(dev|test|stg|prod)` for development, test, staging, production.  

**ApplicationStackCode**  
`([a-z0-9\-]+)` for the application stack that runs within the VPC network.  

### RegExp
`^security-group-(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)-(dev|test|stg|prod)-([a-z0-9\-]+)$`

### Default Pattern Examples
`security-group-ap-northeast-1-prod-web-app-stack`  
`security-group-ap-northeast-2-dev-big-data-stack`  



## EC2 Instance Naming Conventions
### Default Pattern Format
`ec2-RegionCode-EnvironmentCode-ApplicationCode`

### Default Pattern Components
**Region Code**  
`(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)` etc.  

**EnvironmentCode**  
`(dev|test|stg|prod)` for development, test, staging, production.  

**ApplicationStackCode**  
`([a-z0-9\-]+)` for the application stack that runs within the VPC network.  

### RegExp
`^ec2-(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)-(dev|test|stg|prod)-([a-z0-9\-]+)$`

### Default Pattern Examples
`ec2-ap-northeast-1-prod-web-app-stack`  
`ec2-ap-northeast-2-dev-big-data-stack`  

&nbsp;
&nbsp;

## PEM Key Naming Conventions
### Default Pattern Format
`key-RegionCode-EnvironmentCode-ApplicationCode`

### Default Pattern Components
**Region Code**  
`(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)` etc.  

**EnvironmentCode**  
`(dev|test|stg|prod)` for development, test, staging, production.  

**ApplicationStackCode**  
`([a-z0-9\-]+)` for the application stack that runs within the VPC network.  

### RegExp
`^key-(us-east-1|us-west-1|us-west-1|eu-west-1|eu-west-2|eu-central-1| ap-northeast-1|ap-northeast-2|ap-southeast-1|ap-southeast-2)-(dev|test|stg|prod)-([a-z0-9\-]+)$`

### Default Pattern Examples
`key-ap-northeast-1-prod-web-app-stack`  
`key-ap-northeast-2-dev-big-data-stack`  






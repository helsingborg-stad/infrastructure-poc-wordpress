# Infrastructure POC Wordpress
Infrastructure for deployment poc wordpress.

## Cloudformation
### VPC
`aws cloudformation validate-template --template-body file://$PWD/cloudformation/vpc/cfn-stack.yml`
`aws cloudformation create-stack --stack-name infrastructure-poc-wordpress-vpc --template-body file://$PWD/cloudformation/vpc/cfn-stack.yml`
`aws cloudformation update-stack --stack-name infrastructure-poc-wordpress-vpc --template-body file://$PWD/cloudformation/vpc/cfn-stack.yml`
`aws cloudformation delete-stack --stack-name infrastructure-poc-wordpress-vpc`


### ECS
`aws cloudformation validate-template --template-body file://$PWD/cloudformation/ecs/cfn-stack.yml`
`aws cloudformation create-stack --stack-name infrastructure-poc-wordpress-ecs --template-body file://$PWD/cloudformation/ecs/cfn-stack.yml --capabilities CAPABILITY_IAM`
`aws cloudformation update-stack --stack-name infrastructure-poc-wordpress-ecs --template-body file://$PWD/cloudformation/ecs/cfn-stack.yml --capabilities CAPABILITY_IAM`
`aws cloudformation delete-stack --stack-name infrastructure-poc-wordpress-ecs`
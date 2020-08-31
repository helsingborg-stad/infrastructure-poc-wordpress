# Infrastructure POC Wordpress
Infrastructure for deployment poc wordpress.

## Cloudformation
`aws cloudformation create-stack --stack-name infrastructure-poc-wordpress-vpc --template-body file://$PWD/cloudformation/vpc/cfn-stack.yml`
`aws cloudformation create-stack --stack-name infrastructure-poc-wordpress-ecs --template-body file://$PWD/cloudformation/ecs/cfn-stack.yml --capabilities CAPABILITY_IAM`
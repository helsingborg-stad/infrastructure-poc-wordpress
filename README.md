# Infrastructure POC Wordpress


## Cloudformation
`aws cloudformation create-stack --stack-name poc-wp-codepipeline --template-body file://$PWD/cloudformation/vpc/cfn-stack.yml --capabilities CAPABILITY_IAM`
# setup vpc
```
aws cloudformation create-stack --stack-name MyVPCStack --template-body file://vpc-template.yaml
aws cloudformation describe-stacks --stack-name MyVPCStack
```
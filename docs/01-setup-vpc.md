# setup vpc

## build infra
```
aws cloudformation create-stack --stack-name MyVPCStack --template-body file://1-infra-template.yaml
aws cloudformation update-stack --stack-name MyVPCStack --template-body file://1-infra-template.yaml
aws cloudformation validate-template --template-body file://1-infra-template.yaml
aws cloudformation describe-stacks --stack-name MyVPCStack --query "Stacks[0].Outputs"
```

## check stack status
```
aws cloudformation describe-stacks --stack-name MyVPCStack
aws cloudformation describe-stack-events --stack-name MyVPCStack
```

## aws cli useful commands
```
q: quit
space: next page
arrows: scroll
/: search
h: help
```

## delete stack
```
aws cloudformation delete-stack --stack-name MyVPCStack
```
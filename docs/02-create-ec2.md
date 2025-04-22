# setup ec2

## build ec2
```
aws cloudformation create-stack --stack-name MyEC2Stack --template-body file://2-ec2-template.yaml
aws cloudformation update-stack --stack-name MyEC2Stack --template-body file://2-ec2-template.yaml
aws cloudformation validate-template --template-body file://2-ec2-template.yaml
```
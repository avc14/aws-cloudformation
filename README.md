To deploy the stack: 
aws cloudformation deploy --stack-name my-app-stack --template-file cloudformation.yaml  --capabilities CAPABILITY_NAMED_IAM
Note on use of CAPABILITY_NAMED_IAM :
If you have IAM resources with custom names, you must specify CAPABILITY_NAMED_IAM.
In this deployment we are creating IAM role with custom name for lambda, therefore provide CAPABILITY_NAMED_IAM.

# AWS SAM Demos

AWS SAM Demos

# Demo:
https://www.awsclouddemos.com/

# Main Site
https://hexquote.com/


# aws cli commands
aws s3 mb s3://lambda-artifacts-sam

# Package command
aws cloudformation package `
--template-file sam-template.yaml `
--s3-bucket lambda-artifacts-sam `
--output-template-file sam-output-template.yaml

# Deploy command
aws cloudformation deploy `
--template-file sam-output-template.yaml `
--stack-name my-serverless-app-sam `
--capabilities CAPABILITY_IAM

# Delte Stack
aws cloudformation delete-stack `
--stack-name my-serverless-app-sam

# git tags commands
git tag -a 'init' -m 'starting point' HEAD
git push --tags
git tag -l







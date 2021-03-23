# terraform-serverless-node
Simple api gateway lambda integration deployed with terraform.
Follows guide on: https://learn.hashicorp.com/tutorials/terraform/lambda-api-gateway?in=terraform/aws

### How to run

`aws s3api create-bucket --bucket=terraform-serverless-example-neiltest --create-bucket-configuration LocationConstraint=eu-west-1`

`aws s3 cp example.zip s3://terraform-serverless-example-neiltest/v1.0.0/example.zip`

`terraform apply -var="app_version=1.0.0"`
# Terraform an IAM in AWS

## Examples

For examples how to use, please refer to the examples folder.

## AWS Credentials

Set the following environment variables:
```bash
export AWS_ACCESS_KEY_ID=""
export AWS_SECRET_ACCESS_KEY=""
export AWS_DEFAULT_REGION="us-west-2"
```

Refer to: https://www.terraform.io/docs/providers/aws/index.html

## Usage

```
module "iam" {

  source = "john-morsley/aws-iam"

  name = "example"

  tags = {
    Terraform = "true"
  }

}
```
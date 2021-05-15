
![Build](https://github.com/tylangesmith/cdk-bootstrap/actions/workflows/deploy.yml/badge.svg?branch=master)

# CDK Bootstrap

To be able to use [AWS CDK](https://docs.aws.amazon.com/cdk/latest/guide/home.html) we first need to deploy some dependencies which allow CDK to operate in our respective accounts.

Check out the [official CDK bootstrapping documentation](https://docs.aws.amazon.com/cdk/latest/guide/bootstrapping.html)

## Deployment

To deploy this repository there are a few repository secrets that we need to set. To add secrets against the repository checkout the [official documentation](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository) on how to achieve this.

These secret variables are:

| Variable              | Description                    |
|-----------------------|--------------------------------|
| ACCOUNT_ID            | The AWS Account ID             |
| AWS_ACCESS_KEY_ID     | The IAM user Access Key ID     |
| AWS_SECRET_ACCESS_KEY | The IAM user Secret Access Key |

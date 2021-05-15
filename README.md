
![Build](https://github.com/tylangesmith/cdk-bootstrap/actions/workflows/deploy.yml/badge.svg?branch=master)

# CDK Bootstrap

To be able to use [AWS CDK](https://docs.aws.amazon.com/cdk/latest/guide/home.html) we first need to deploy some dependencies which allow CDK to operate in our respective accounts.

Check out the [official CDK bootstrapping documentation](https://docs.aws.amazon.com/cdk/latest/guide/bootstrapping.html)

## Deploy to Multiple Regions

```yml{1}
steps:
  - uses: actions/checkout@v2
  - uses: actions/setup-node@v2
    with:
      node-version: '14'
  - run: ./bootstrap.sh
    env:
      AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
      AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
      REGION: ap-southeast-2
```



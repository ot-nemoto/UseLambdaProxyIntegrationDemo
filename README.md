# UseLambdaProxyIntegrationDemo 

## デプロイ

Lambdaプロキシ統合を使用したAPI Gateway

```sh
aws cloudformation create-stack \
    --stack-name use-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://use-lambda-proxy-integration-template.yaml
```

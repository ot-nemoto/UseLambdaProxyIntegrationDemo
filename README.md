# UseLambdaProxyIntegrationDemo 

## デプロイ

```sh
aws cloudformation create-stack \
    --stack-name use-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://template.yaml
```

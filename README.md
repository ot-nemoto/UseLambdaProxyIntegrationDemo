# UseLambdaProxyIntegrationDemo 

## 概要

- API GatewayとLambda関数を使ったサーバレス環境のサンプルを構築します

## デプロイ

Lambdaプロキシ統合を使用したAPI Gateway

```sh
aws cloudformation create-stack \
    --stack-name use-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://use-lambda-proxy-integration-template.yaml
```

Lambdaプロキシ統合を使用しないAPI Gateway

```sh
aws cloudformation create-stack \
    --stack-name unuse-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://unuse-lambda-proxy-integration-template.yaml
```

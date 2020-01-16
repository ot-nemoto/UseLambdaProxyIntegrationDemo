# UseLambdaProxyIntegrationDemo 

## 概要

- API GatewayとLambda関数を使ったサーバレス環境のサンプルを構築します

## デプロイ

### use-lambda-proxy-integration-demo

- Lambdaプロキシ統合を使いAPI GatewayとLambdaを連携させる構成の構築

![use-lambda-proxy-integration-demo](https://github.com/ot-nemoto/UseLambdaProxyIntegrationDemo/blob/images/UseLambdaProxyIntegrationDemo-use-lambda-proxy-integration-demo.png)

```sh
aws cloudformation create-stack \
    --stack-name use-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://use-lambda-proxy-integration-template.yaml
```

### unuse-lambda-proxy-integration-demo

- Lambdaプロキシ統合に合わせたLambdaに対して、Lambdaプロキシ統合を使わずAPI GatewayとLambdaを連携させる構成の構築
- エラー時ののハンドリングには未対応

![unuse-lambda-proxy-integration-demo](https://github.com/ot-nemoto/UseLambdaProxyIntegrationDemo/blob/images/UseLambdaProxyIntegrationDemo-unuse-lambda-proxy-integration-demo.png)

```sh
aws cloudformation create-stack \
    --stack-name unuse-lambda-proxy-integration-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://unuse-lambda-proxy-integration-template.yaml
```

### unuse-lambda-proxy-integration-ex-demo

- Lambdaプロキシ統合に合わせたLambdaに対して、Lambdaプロキシ統合を使わずAPI GatewayとLambdaを連携させる構成の構築
- エラー時のハンドリングにも対応

![unuse-lambda-proxy-integration-ex-demo](https://github.com/ot-nemoto/UseLambdaProxyIntegrationDemo/blob/images/UseLambdaProxyIntegrationDemo-unuse-lambda-proxy-integration-ex-demo.png)

```sh
aws cloudformation create-stack \
    --stack-name unuse-lambda-proxy-integration-ex-demo \
    --capabilities CAPABILITY_NAMED_IAM \
    --template-body file://unuse-lambda-proxy-integration-ex-template.yaml
```

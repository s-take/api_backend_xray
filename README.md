# api_backend_xray

install package

```
$npm install aws-xray-sdk
```

```
$aws cloudformation package \
    --template-file template.yaml \
    --output-template-file serverless-output.yaml \
    --s3-bucket <bucket>
```

```
$aws cloudformation deploy 
    --template-file ./serverless-output.yaml \
    --stack-name api-backend-xray \
    --capabilities CAPABILITY_IAM
```

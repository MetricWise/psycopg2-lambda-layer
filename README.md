# psycopg2-lambda-layer

https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/building-layers.html

```bash
sam build --use-container
cd .aws-sam/build/Psycopg2Layer
zip -r ../psycopg2.zip *
cd -
aws lambda publish-layer-version --compatible-runtimes python3.9 --layer-name psycopg2 --zip-file fileb://.aws-sam/build/psycopg2.zip
```

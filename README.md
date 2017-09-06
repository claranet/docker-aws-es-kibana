# aws-es-kibana Docker image

Run [aws-es-kibana](https://github.com/santthosh/aws-es-kibana) inside [Docker](https://www.docker.com/).

## Docker Hub

[https://hub.docker.com/r/claranet/aws-es-kibana/](https://hub.docker.com/r/claranet/aws-es-kibana/)

## Usage

```shell
docker run -e AWS_SESSION_TOKEN -e AWS_ACCESS_KEY_ID -e AWS_SECRET_ACCESS_KEY -e AWS_DEFAULT_REGION -p 9200:9200 claranet/aws-es-kibana <domain-endpoint>
```

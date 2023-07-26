# aws-terraform-k8s-cli Container

## Synopsis

aws-terraform-k8s-cli is designed for ci/cd propose.
```
terraform 
aws-cli 
git
kubectl
```

## Running Locally

### Requirements
- Docker

### Building & Running Locally
```
docker build -t brpedromaia/aws-terraform-k8s-cli:local . -f ContainerFile
docker run --rm -it --name aws-terraform-k8s-cli \
 -v $PWD:/sync/ \
 brpedromaia/aws-terraform-k8s-cli:local sh
```

### Running Container Image
```
docker run --rm -it --name aws-terraform-k8s-cli \
 -v $PWD:/sync/ \
 brpedromaia/aws-terraform-k8s-cli:v1 sh
```

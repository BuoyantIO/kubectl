[![Docker Pulls](https://img.shields.io/docker/pulls/buoyantio/kubectl.svg)](https://hub.docker.com/r/buoyantio/kubectl/)

# Kubectl

Kubectl in a scratch Docker image.

Available at: https://hub.docker.com/r/buoyantio/kubectl/

## Run

```bash
docker run buoyantio/kubectl:latest
```

## Build

```bash
docker build -t buoyantio/kubectl:latest .
```

Build latest stable Kubernetes version

```bash
K8S_VERSION=$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)
docker build -t buoyantio/kubectl:$K8S_VERSION --build-arg K8S_VERSION=$K8S_VERSION .
```

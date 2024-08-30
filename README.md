# ALE

ALE is a Kubernetes-based developer platform that offers developer self-service capabilities and supports functionality extensions through plugins.



## Documentation

A detailed installation and configuration guide is available in the [ALE Docs](https://docs.ale.run/).



## Getting Started

To install ALE, you’ll need the following:

- Kubernetes version 1.24 or higher
- A private registry with read and write access
- Ingress and Cert Manager
- Storage class

### Installation

1. Use the following command to install ALE on Kubernetes.

```sh
$ kubectl apply -f https://raw.githubusercontent.com/ale-run/ale/main/k8s/v1.1.0/ale.yaml
```

2. Access the operating system.

```sh
$ kubectl port-forward deployment/ale-operator 9999:80 -n ale
```


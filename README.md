 # KEDA Poc
This repository demonstrates a Proof of Concept (PoC) for using Kubernetes Event-Driven Autoscaling (KEDA) to scale applications based on RabbitMQ queue size. It includes setup instructions for deploying KEDA, configuring RabbitMQ, and automating scaling of consumer workloads in a Kubernetes cluster. The project aims to showcase how KEDA can trigger automatic scaling based on message queue length in RabbitMQ.
 ## Prerequisites
 - have kubernetes cluser

## Create Kind cluster
```shell
kind create cluster --name keda-cluster
```

 ## Install Keda using helm

 To deploy KEDA with Helm:

1. Add Helm repo
```shell

helm repo add kedacore https://kedacore.github.io/charts
```
2. Update Helm repo
```shell
helm repo update
```
3. Install keda Helm chart

```shell
helm install keda kedacore/keda --namespace keda --create-namespace
```

## Install RabbitMQ Queue Scaler
N/A

## Deploy the app

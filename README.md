 # KEDA Poc

 ## Prerequisites
 - have kubernetes cluser


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
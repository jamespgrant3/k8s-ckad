# Notes 

## Network Policy
- can be though of as a Security Group for pods.

## kubectl
- create resources on the fly using `kubectl run`
- supply nested config using commas:
```
kubectl run quota my-quoate --hard=cpu=1,memory=1G
```
This will add a config for `hard`, with two properties: `cpu` and `memory`.
- get resources in all namespaces using `-A`.
```
kubectl get pods -A
```

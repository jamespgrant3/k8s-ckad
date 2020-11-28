# Overview
This example demonstrates how a `PersistentVolume` can be used for persistent, cross-pod, data storage.

# Instructions:
Run the following commands:

- `kubectl apply -f ./data-volume.yml`
- `kubectl apply -f ./data-volume-claim.yml`
- `kubectl apply -f ./writer-pod.yml`
- `kubectl apply -f ./reader-pod.yml`
- `kubectl logs reader-pod`

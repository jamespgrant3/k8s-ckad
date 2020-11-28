# Overview
This example demonstrates that without a `NetworkPolicy`, pods can communicate with one another.

# Instructions:
Run the following commands:
- `kubectl apply -f ./web-pod.yml`
- `kubectl apply -f ./data-pod.yml`
- `kubectl apply -f ./data-pod-svc.yml`
- `kubectl exec web-pod -- curl data-pod-svc:8080`

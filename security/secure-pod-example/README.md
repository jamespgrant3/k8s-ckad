# Overview
This example demonstrates that with a `NetworkPolicy`, pods communicate can be restricted.

# Instructions:
Run the following commands:
- `kubectl apply -f ./approved-web-pod.yml`
- `kubectl apply -f ./unapproved-web-pod.yml`
- `kubectl apply -f ./data-pod.yml`
- `kubectl apply -f ./data-pod-svc.yml`
- `kubectl apply -f ./data-pod-policy.yml`
- `kubectl exec approved-web-pod -- curl data-pod-svc:8080`
- `kubectl exec unapproved-web-pod -- curl data-pod-svc:8080`

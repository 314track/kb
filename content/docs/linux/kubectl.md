---
title: "kubectl"
draft: false
---

# kubectl

```bash
kubectl apply -f <file> [-f <file>]...
```

## Apply a configuration

```bash
kubectl apply -f https://k8s.io/examples/admin/dns/dnsutils.yaml -n <namespace>
```

## List pods in a specific namespace

```bash
kubectl get pods -n <namespace>
```

## delete a pod

```bash
kubectl delete pods/dnstest -n <namespace>
```

## Run container with specific name in a specific namespace

```bash
kubectl run dnstest --image registry.k8s.io/e2e-test-images/agnhost:2.39 -n <namespace>
```

## Or interactive

```bash
kubectl run dnstest --image registry.k8s.io/e2e-test-images/agnhost:2.39 -it - n <namespace>
```

## Execute command directly in container

```bash
kubectl exec <pod name> -n <namespace> -- curl -Iv http://<url>
```

```bash
kubectl exec <pod name> -- netstat -anp | grep 8080
```

# Create First cluster:
```
kind create cluster # Default cluster context name is `kind`.

```

# Create custom named cluster:
```

kind create cluster --name kind-2

```

# To access clusters:

```

kubectl get pods -A  --context kind-kind

```

```

kubectl get pods -A  --context kind-kind-2

```


# Create First cluster:
```
kind create cluster # Default cluster context name is `kind`.

```

# Create custom named cluster:
```

kind create cluster --name kind-2

```

# Create custom configured cluster by passing config file:
```
kind create cluster --config config_file.yaml --kubeconfig /path/to/the/kubeconfig/file

```

For example:

```
kind create cluster --config c1.yaml --kubeconfig /home/ubuntu/work/kind/.kind/config

```

# To access clusters:

```

kubectl get pods -A  --context kind-kind

```

```

kubectl get pods -A  --context kind-kind-2

```


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

kubectl cluster-info kind-{name_of_cluster} --kubeconfig path/to/kubeconfig

```

For example:


```

kubectl cluster-info --context kind-kind --kubeconfig /home/ubuntu/work/kind/.kind/config


```

```

kubectl cluster-info --context kind-kind-2 --kubeconfig /home/ubuntu/work/kind/.kind2/config

```


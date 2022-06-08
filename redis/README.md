# Kubernetes Redis Cluster
### Create Persistent Volumes

```
kubectl create -f persistentvolume
```

### Create Persistent Volumes Claims

```
kubectl create -f persistentvolumeclaims
```

### Create Redis Cluster Configuration

```
kubectl create configmap redis-conf --from-file=redis.conf
```

### Create Redis Services

```
kubectl create -f statefulset-services/redis-headless.yaml
```

### Create Redis Statefulset

```
kubectl create -f statefulset/redis-statefulset.yaml
```



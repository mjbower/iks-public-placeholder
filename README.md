# iks-public-placeholder

## Helm 3 install
`helm install mjbtest ./iks-tp-stack`

## Helm 3 delete
`helm delete mjbtest ./iks-tp-stack`

## Exec into the first pod

```
kubectl exec -it $(kubectl get pods --selector app=mjbtest -o jsonpath='{.items[*].metadata.name}') -- bash
```


## ServiceAccount 
tokens created in /var/run/secrets/


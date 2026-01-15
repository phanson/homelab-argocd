# BookLore

Pre-create secret with passwords:

```
kubectl create secret -n booklore generic booklore-passwords --from-literal=DB_PASSWORD=changeme --from-literal=MYSQL_ROOT_PASSWORD=itsasecret
```

Order of operations:
- namespace
- secret
- pv-*
- pvc-*
- configmap
- deployment
- service
- ingress
# micro-arch-k8s
# приложение отвечает на arch.homework/health (добавить запись в hosts)

## Развёртывание: 
```bash
minikube start
```

```bash
minikube dashboard
```

```bash
helm install social-net social-net-chart
```

```bash
minikube tunnel
```

## Можно поэкспериментировать с переключением версий и работой RollingUpdate:
  
```bash
kubectl -n social-net set image deployment/golang-app golang-app=van4ik/social-net:1.0.4
```

```bash
kubectl -n social-net set image deployment/golang-app golang-app=van4ik/social-net:1.0.3
```



# linuxtips-multirao-k8s

## Dia 2

```
k run nginx --image nginx --port 80

k expose pod nginx # implicit ClusterIp
k expose pod nginx --type NodePort
k expose pod nginx --type LoadBalancer

k delete services nginx

k exec -ti nginx -- bash

kubectl port-forward service/nginx 8080:80

echo "giropops strigus girus" > usr/share/nginx/html/index.html

k create deployment giropops --image nginx --port 80 --replicas 3

k scale deployment giropops --replicas 5

k expose deployment giropops --type NodePort

kubectl port-forward service/giropops 8080:80
```

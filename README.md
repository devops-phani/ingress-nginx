# ingress-nginx

Install the ingress-nginx using helm

```
helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace
```

Install the ingress-nginx using kubernetes manifest files

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.0/deploy/static/provider/cloud/deploy.yaml
```

Reference link:

https://kubernetes.github.io/ingress-nginx/deploy/

Check the pods

```
kubectl get pods --namespace=ingress-nginx
```

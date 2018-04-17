# Kubernetes Samples

## Kubernetes commands

```
kubectl version
kubectl logs podName
kubectl explain pods
kubectl create -f fileName.yml
kubectl get pods --namespace=kube-system
kubectl logs name -c containerName
kubectl describe pods podName
kubectl get rc
kubectl edit rc nginx
kubectl delete rc nginx
kubectl run nginx --image=nginx:1.12.0 --replicas=2 --port=80
kubectl expose deployment nginx --port=80 --target-port=80
kubectl replace -f nginxDeployment.yml
kubectl apply -f nginxDeployment.yml
kubectl set image deployment nginx nginx=nginx:1.13.1
```

General spec:

```yml
apiVersion: Kubernetes API version
kind: object type
metadata: 
  spec metadata, i.e. namespace, name, labels and annotations
spec: 
  the spec of Kubernetes object

```
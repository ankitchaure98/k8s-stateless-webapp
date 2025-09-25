# k8s-stateless-webapp
Deploy App on Kuberenetes

## Features
- Deployment with 3 replicas
- ConfigMap for environment variables
- ClusterIP Service exposing port 80
- Horizontal Pod Autoscaler (HPA) scaling 3–10 pods based on CPU > 70%

## Apply Manifests
Run the following commands in order:

# bash
kubectl apply -f configmap.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa.yaml


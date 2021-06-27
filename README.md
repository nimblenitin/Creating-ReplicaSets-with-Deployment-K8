# Creating-ReplicaSets-with-Deployment-K8
A Deployment is a higher-level concept that manages ReplicaSets and provides declarative updates to Pods along with a lot of other useful features

Simple example to create ReplicaSets with Deployment in Declarative method with YAML
Steps followed-

*As Root*
```

1. Run below dry run command to auto create YAML
kubectl create deployment nginx-deployment --image=nginx:1.19.0 --replicas=5 --dry-run -o yaml


2. Create the YAML file with YAML output from above command
vim deploy.yaml 
      
3. Run the YAML-
kubectl apply -f deploy.yaml
 
3. View the Pod created:
kubectl get pods -o wide
 
 ```
*As Root*

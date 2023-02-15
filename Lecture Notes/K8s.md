## K8s 

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem

- Flippy => simple app with hello world lies in the hosted server and shared her environment with other scary apps (She needs home)

## The Environment: 
- A home: a boat but in the middle of the ocean 
## Containers:
- K8s - 100 of containers
`Namespace to identify things`
## Containers to Pod: 
- POD = runnable unit of work.. 
- K8s will take care of connecting your pod to network and rest of the k8s ecosystem.. 

## Dind-cluster (Docker cluster in cluster K8s setup)

```bash
wget https://cdn.rawgit.com/kubernetes-sigs/kubeadm-dind-cluster/master/fixed/dind-cluster-v1.12.sh
```

### K8s Basic commands:

```bash
Chmod +x 

./dind-cluster-v1.12.sh 

Kubectl get all
Kubectl get nodes (master & slave)
Kubectl get pods 
Kubectl create deployment tomcat —image=tomcat 
Kubectl get pods -w (watch)
Kubectl get rs (replica sets)
Kubectl get pods -n kube-system (name space)
Kubectl scale —replicas=5 deployment/tomact
Kubectl delete deployment/tomcat  
Kubectl expose deployment hello  - - type=NodePort - - port=8080 
Kubectl get services 
Kubectl scale deployment/hello  - - replicas=3
Kubectl describe pods 
Kubectl delete pod/pod name
kubectl run hello-kubernetes --replicas=3 --image=paulbouwer/hello-kubernetes:1.5 --port=8080 --env="MESSAGE=I just deployed this on Kubernetes!"
kubectl expose deployment hello-kubernetes --type=LoadBalancer --port=80 --target-port=8080 --name=hello-kubernetes
kubectl set image deployments/kubernetes-bootcamp deployment=image:tag
kubectl rollout undo deployments/kubernetes-bootcamp
```
- When fails -> Kubectl -> controller manager -> api server -> scheduler -> create pods -> get the nodes 
- Docker exec -it kube-master bash 
- Etcd -> redis mathiri 
- Deployment -> replica controller -> pods -> container -> environment 

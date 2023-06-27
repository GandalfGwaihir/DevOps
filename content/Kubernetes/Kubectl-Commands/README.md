![](https://geekflare.com/wp-content/uploads/2021/03/kubectl.jpg)

## [kubectl](https://kubernetes.io/docs/reference/kubectl/) is a command-line tool used for interacting with Kubernetes clusters. It allows users to create, inspect, update, and delete Kubernetes resources like pods, deployments, services, and more, from the command line.

The Kubectl command follows a simple syntax:
```bash 
kubectl [action] [resource] [name] [flags]. 
```
---
# Useful Commands

### Basic Commands

* List resources
```bash
kubectl get [resource]
```
* Show detailed information about a resource
```bash
kubectl describe [resource] [name]
```
* Create a new resource
```bash
kubectl create [resource] [name]
```
* Delete a resource
```bash
kubectl delete [resource] [name]
```
* Apply a configuration file to create or update a resource
```bash
kubectl apply -f [filename] 
```
* Edit a resource in real-time
```bash
kubectl edit [resource] [name]
```
---
### Cluster Management Commands
* Show cluster information
```bash
kubectl cluster-info 
```
* List all nodes in the cluster
```bash
kubectl get nodes
```
* Show detailed information about a node
```bash
kubectl describe node [name]
```
* List all namespaces in the cluster
```bash
kubectl get namespaces
```
* Create a new namespace
```bash
kubectl create namespace [name]
```
* View and modify kubectl configuration settings
```bash
kubectl config view
```
* Show client and server version information
```bash
kubectl version
```
* List all available API resources
```bash
kubectl api-resources
```
---
### Advanced Commands

* Show logs for a pod
```bash
kubectl logs [pod]
```
* Run a command inside a running pod
```bash
kubectl exec -it [pod] [command]
```
* Forward a local port to a port on a pod
```bash
kubectl port-forward [pod] [local port]:[remote port]
```
* Manage rollouts for a resource
```bash
kubectl rollout [resource] [name]
```
* Scale the number of replicas for a resource
```bash
kubectl scale [resource] [name] --replicas=[num]
```
* Show resource usage statistics
```bash
kubectl top [resource] [name]
```
* Run a one-time command in a new pod
```bash
kubectl run [name] --image=[image name]
```
* Show detailed documentation for a resource
```bash
kubectl explain [resource]
```

### As always, you can use the ```kubectl --help``` command or check out the official Kubernetes documentation for more information.
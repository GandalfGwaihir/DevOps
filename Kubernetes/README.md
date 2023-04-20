![Kubernetes Logo](https://kubernetes.io/images/kubernetes-horizontal-color.png)


### [Kubernetes](https://kubernetes.io), also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications.
---

## Kubernetes Cluster

![Kubernetes Cluster](https://d33wubrfki0l68.cloudfront.net/2475489eaf20163ec0f54ddc1d92aa8d4c87c96b/e7c81/images/docs/components-of-kubernetes.svg)

A Kubernetes cluster is a group of nodes that work together to run containerized applications. The cluster consists of a control plane and worker nodes.

---

* Control Plane

The control plane manages the overall state of the cluster, including scheduling and scaling of applications, monitoring and logging, and networking. The control plane consists of  Kubernetes API server, etcd, kube-scheduler, kube-controller-manager, and cloud-controller-manager.

---

* Worker Nodes

The worker nodes are responsible for running the containers and executing the tasks assigned by the control plane. Each worker node runs a container runtime, such as Docker, and a Kubernetes agent called kubelet, which communicates with the control plane to receive instructions.




# kubernaties-training

- Kubernaties default don't have any network inteface so we can use calico.
- It also don't have deafult LB so we can use metalLB

- Basics:
Kubernetes Cluster: A set of nodes (servers) that run containerized applications.
kubectl Commands (Command Line Interface for Kubernetes):
Cluster Info:

kubectl cluster-info: Display cluster information.
Nodes:

kubectl get nodes: List all nodes in the cluster.
kubectl describe node <node-name>: Get detailed information about a specific node.
Pods:

kubectl get pods: List all pods in the default namespace.
kubectl get pods -n <namespace>: List pods in a specific namespace.
kubectl describe pod <pod-name>: Get detailed information about a specific pod.
Deployments:

kubectl get deployments: List all deployments.
kubectl describe deployment <deployment-name>: Get detailed information about a specific deployment.
Services:

kubectl get services: List all services.
kubectl describe service <service-name>: Get detailed information about a specific service.
Logs and Debugging:

kubectl logs <pod-name>: Display logs from a pod.
kubectl exec -it <pod-name> -- /bin/sh: Start an interactive shell in a pod.
Scaling:

kubectl scale deployment <deployment-name> --replicas=<desired-replica-count>: Scale a deployment.
Port Forwarding:

kubectl port-forward <pod-name> <local-port>:<pod-port>: Forward ports from a pod to your local machine.
Deleting Resources:

kubectl delete <resource-type> <resource-name>: Delete a specific resource.
Concepts:
Pod:

The smallest deployable unit in Kubernetes, typically containing one or more containers.
Deployment:

Manages the lifecycle of pods, ensuring a desired number of replicas are running.
Service:

Exposes pods to network traffic, either within the cluster or externally.
Namespace:

A virtual cluster that provides isolation and resource segregation within a physical cluster.
ReplicaSet:

Ensures a specified number of replicas of a pod are running at all times.
Ingress:

Manages external access to the services in a cluster.
ConfigMap and Secret:

Store configuration data and sensitive information separately from the application code.
Volume:

Provides a way to store and share data between containers in a pod.
Namespace:

A way to divide cluster resources between multiple users or teams.
Remember, this cheatsheet provides a high-level overview. Kubernetes is a complex system with many more concepts and commands to explore. It's recommended to refer to the official Kubernetes documentation for in-depth information and updates.

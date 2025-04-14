## Get
1. Get pod names in the default namespace:
   ```shell
   kubectl get pods -n default
   ```

2. Get persistent volume claim status:
   ```shell
   kubectl get pvc
   ```

3. Get all services:
   ```shell
   kubectl get services
   ```

4. Get deployments in a namespace:
   ```shell
   kubectl get deployments -n <namespace>
   ```

5. Get nodes in the cluster:
   ```shell
   kubectl get nodes
   ```

6. Get details of a specific resource:
   ```shell
   kubectl describe <resourceType> <resourceName>
   ```

## Execute
1. Look inside a Kubernetes pod (open a shell):
   ```shell
   kubectl exec -it <pod-name> -- /bin/bash
   ```

2. Run a single command in a pod:
   ```shell
   kubectl exec <pod-name> -- <command>
   ```
## Debug
1. Describe a problem in a pod:
   ```shell
   kubectl describe pod <pod-name>
   ```

2. View logs of a specific pod:
   ```shell
   kubectl logs <pod-name>
   ```

3. Follow live logs of a pod:
   ```shell
   kubectl logs -f <pod-name>
   ```

4. Debug a container in a pod:
   ```shell
   kubectl exec -it <pod-name> --container <container-name> -- /bin/bash
   ```

## Storage

1. Get storage classes in the cluster:
   ```shell
   kubectl get storageclass
   ```

2. Get persistent volumes in the cluster:
   ```shell
   kubectl get pv
   ```

## Create
1. Create a resource from a YAML file:
   ```shell
   kubectl apply -f <file.yaml>
   ```

2. Create a namespace:
   ```shell
   kubectl create namespace <namespace-name>
   ```

3. Expose a deployment as a service:
   ```shell
   kubectl expose deployment <deployment-name> --type=<service-type> --port=<port>
   ```
   ## Delete
1. Delete a pod:
   ```shell
   kubectl delete pod <pod-name>
   ```

2. Delete a namespace:
   ```shell
   kubectl delete namespace <namespace-name>
   ```

3. Delete a resource using a YAML file:
   ```shell
   kubectl delete -f <file.yaml>
   ```

## Miscellaneous
1. Scale a deployment:
   ```shell
   kubectl scale deployment <deployment-name> --replicas=<number>
   ```

2. Apply changes to a resource:
   ```shell
   kubectl apply -f <file.yaml>
   ```

3. View cluster information:
   ```shell
   kubectl cluster-info
   ```

4. Check resource usage:
   ```shell
   kubectl top nodes
   kubectl top pods
   ```

5. Set a context for kubectl commands:
   ```shell
   kubectl config use-context <context-name>
   ```

6. View current context:
   ```shell
   kubectl config current-context
   ```

## IPID

1. See the Pods:
   ```shell
   kubectl get pods -n ipid
   ```
2. Restart all the Pods:
   ```shell
   kubectl delete pods --all -n ipid
   ```

# Sample_CKAD_Questions
Sample_CKAD_Questions and answers

Here are 50 real hard CKAD questions across all concepts to practice:
Create a namespace called ckad-practice and make sure that the pod count in the namespace is not more than 10.
Create a deployment called nginx-deployment with image nginx:1.14.
Create a service called nginx-service that will drive traffic to the deployment.
Update the deployment to nginx:latest using a canary deployment update strategy.
Add labels to the deployment as upgrade=canary.
Redirect 60% of the incoming traffic to the old deployment and 40% of the incoming traffic to the new deployment.
Create two pods, one with the image nginx:1.14 and the other with the image busybox:latest.
Control the traffic between these two pods, such that access to the nginx server is only allowed from the busybox pod and the busybox pod is free to access or to be accessed from anywhere.
Create a secret called my-secret with the following key-value pairs:
username = admin
password = secret
Create a configmap called my-configmap with the following content:
apiVersion: v1
data:
  my-key: my-value

Create a pod that uses the my-secret secret and the my-configmap configmap.
Create a persistent volume called my-pv with the following storage class:
apiVersion: storage.k8s.io/v1
kind: StorageClass
metadata:
  name: my-storage-class
provisioner: kubernetes.io/gce-pd
parameters:
  type: pd-standard

Create a persistent volume claim called my-pvc that uses the my-storage-class storage class.
Create a pod that uses the my-pvc persistent volume claim.
Create a Job called my-job that runs the command echo "hello world".
Create a CronJob called my-cronjob that runs the command echo "hello world" every minute.
Create a DaemonSet called my-daemonset that runs the nginx image on all nodes in the cluster.
Create a StatefulSet called my-statefulset that runs 3 nginx pods, each with a unique name.
Create a Headless Service called my-headless-service that exposes the pods in the my-statefulset StatefulSet.
Create a NetworkPolicy called my-networkpolicy that allows only pods in the my-namespace namespace to access the pods in the my-statefulset StatefulSet.
Create a HorizontalPodAutoscaler called my-hpa that automatically scales the my-deployment deployment up or down based on the CPU usage of the pods.
Create a Ingress called my-ingress that exposes the pods in the my-deployment deployment to the outside world.
Create a PrometheusRule called my-prometheusrule that alerts on the CPU usage of the pods in the my-deployment deployment.
Create a ServiceMonitor called my-servicemonitor that monitors the pods in the my-deployment deployment and sends metrics to Prometheus.
Create a PodDisruptionBudget called my-poddisruptionbudget that ensures that there are always at least 2 pods running in the my-deployment deployment.
Create a ClusterRoleBinding called my-clusterrolebinding that gives the my-user user the my-role role in the cluster.
Create a ClusterRole called my-clusterrole that allows the my-role role to do the following:
Create pods
Delete pods
Get pods
List pods
Create a Role called my-role that allows the my-user user to do the following:
Create pods in the my-namespace namespace
Delete pods in the my-namespace namespace
Get pods in the my-namespace namespace
List pods in the my-namespace namespace
Create a RoleBinding called my-rolebinding that gives the my-user user the my-role role in the my-namespace namespace

Create a pod that has a liveness probe that checks the HTTP status code of the /health endpoint.
Create a pod that has a readiness probe that checks the number of pods in the my-deployment deployment.
Create a pod that has a startup probe that checks the CPU usage of the pod.
Create a pod that uses the my-secret secret and the my-configmap configmap, and mount them as volumes.
Create a pod that uses a persistent volume claim to access a persistent volume.
Create a pod that uses a Job to run a command.
Create a pod that uses a CronJob to run a command at a specific time.
Create a pod that uses a DaemonSet to run on all nodes in the cluster.
Create a pod that uses a StatefulSet to run with a unique name.
Create a pod that uses a Headless Service to expose its IP address.
Create a pod that uses a NetworkPolicy to control the traffic to and from it.
Create a pod that uses a HorizontalPodAutoscaler to automatically scale up or down based on the CPU usage.
Create a pod that uses an Ingress to expose it to the outside world.
Create a pod that uses a PrometheusRule to alert on metrics.
Create a pod that uses a ServiceMonitor to send metrics to Prometheus.
Create a pod that uses a PodDisruptionBudget to ensure that there are always a minimum number of pods running.
Create a pod that uses a ClusterRoleBinding to give a user a role in the cluster.
Create a pod that uses a ClusterRole to give a role to a user in the cluster.
Create a pod that uses a Role to give a user a role in a namespace.
Create a pod that uses a RoleBinding to give a user a role in a namespace.
Create a pod that uses a pod template to create a new pod.

# ckad-practice

## Question 1

Create a new deployment named nginx with below parameters:
- Run the deployment in the frontend namespace
- Configure with 5 replicas
- Configure the pod with a container image of nginx:1.18.0-alpine
- Set an environment variable of NGINX_PORT= 8080 and also expose that port for the container above


## Question 2
A project that you are working on has a requirement for persistent data to be available.
Task To facilitate this, perform the following tasks:
-  Create a file on node master at /opt/q2/data/index.html with the content
Acct=Finance
- Create a PersistentVolume named task-pv-volume using hostPath and allocate 1Gi to it, specifying
that the volume is at /opt/q2/data/ on the cluster's node. 
- The configuration should specify the access mode of ReadWriteOnce . 
- It should define the StorageClass name q2 for the PersistentVolume , which will be used to bind PersistentVolumeClaim requests to this PersistenetVolume.

## Question 3

- Create a namespace called falcon and a pod with image nginx called q1-nginx in this namespace, and allow traffic on port 80.
- Get information about the pod, save output to a file named /tmp/pod-q1-nginx.out.
- Get pod logs, save to a file named /tmp/q1-nginx.log.
- Execute command curl localhost:80 on the nginx pod, save output to a file named /tmp/q1-cmd.out.
- Set namespace falcon as the default namespace. View config to verify it and save output to a fil named /tmp/config-namespace.out.

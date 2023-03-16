# Exercise 11

The content overlaps with the curriculum of the CKAD exam. You can find the instructions and the solution in the exercises folder of the GitHub repository [bmuschko/ckad-crash-course](https://github.com/bmuschko/ckad-crash-course/blob/master/exercises/15-service/instructions.md).

- Create a Service named myapp of type ClusterIP that exposes port 80 and maps to the target port 80.
- Create a Deployment named myapp that creates 1 replica running the image nginx. Expose the container port 80.
- Scale the Deployment to 2 replicas.
- Create a temporary Pod using the image busybox and run a wget command against the IP of the service.
- Change the service type so that the Pods can be reached from outside of the cluster.
- Run a wget command against the service from outside of the cluster.
- (Optional) Discuss: Can you expose the Pods as a service without a deployment?
- (Optional) Discuss: Under what condition would you use the service type LoadBalancer?
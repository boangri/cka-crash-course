# Exercise 5

The content overlaps with the curriculum of the CKAD exam. You can find the instructions and the solution in the exercises folder of the GitHub repository [bmuschko/ckad-crash-course](https://github.com/bmuschko/ckad-crash-course/blob/master/exercises/07-deployment/instructions.md).

- Create a Deployment named deploy with 3 replicas. The Pods should use the nginx image and the name nginx. The Deployment uses the label tier=backend. The Pods should use the label app=v1.
- List the Deployment and ensure that the correct number of replicas is running.
- Update the image to nginx:latest.
- Verify that the change has been rolled out to all replicas.
- Scale the Deployment to 5 replicas.
- Have a look at the Deployment rollout history.
- Revert the Deployment to revision 1.
- Ensure that the Pods use the image nginx.
- (Optional) Discuss: Can you foresee potential issues with a rolling deployment? How do you configure a update process that first kills all existing containers with the current version before it starts containers with the new version?
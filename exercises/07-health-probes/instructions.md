# Exercise 7

The content overlaps with the curriculum of the CKAD exam. You can find the instructions and the solution in the exercises folder of the GitHub repository [bmuschko/ckad-crash-course](https://github.com/bmuschko/ckad-crash-course/blob/master/exercises/08-pod-probes/instructions.md).


In this exercise, you will create a Pod running a NodeJS application. The Pod will define readiness and liveness probes with different parameters.

NOTE: If you do not already have a cluster, you can create one by using minikube or you can use the Katacoda lab "Creating a Pod with a readiness Probe of type HTTP GET request".

- Create a new Pod named hello with the image bmuschko/nodejs-hello-world:1.0.0 that exposes the port 3000. Provide the name nodejs-port for the container port.
- Add a Readiness Probe that checks the URL path / on the port referenced with the name nodejs-port after a 2 seconds delay. You do not have to define the period interval.
- Add a Liveness Probe that verifies that the app is up and running every 8 seconds by checking the URL path / on the port referenced with the name nodejs-port. The probe should start with a 5 seconds delay.
- Shell into container and curl localhost:3000. Write down the output. Exit the container.
- Retrieve the logs from the container. Write down the output.

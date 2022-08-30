# Chaos Engineering with Chaos Mesh.

## Objective:
As a standard objective of this procedure is to enforce some failures in the cluster and see where the vulnerabilities exist.

## Experiment 1 Pod Failure:
As a very standard experiment on the cluster is to force a failure to a pod in a given namespace and see how the cluster reacts in terms of load balancing, and how long will it take until a new pod is created.

## Experiment 1 Results:
The experiment ran for a total of 10s while monitoring the status of the pods one pod indeed failed and another one was created almost immedietly after. during the downtime one could still access the website.

## Experiment 2 Kernel Failure:
Forcing a failure in the kernel and seeing how to cluster reacts.

## Experiment 2 Results:
The experiment ran by forcing a failure on the kernel of the cluster. During the downtime of the cluster which was very minor (a couple of seconds). The cluster was surprisingly still working and the website could still be reached.

## Experiment 3 Pod Kill:
This experiment will kill a pod inside of the cluster in a given namespace.

## Experiment 3 Results:
After killing all pods/fixed number of pods in a given namespace, the pods are almost immedietly created (less than a couple of seconds)
#Chaos Engineering with Chaos Mesh.#

##Objective:##
As a standard objective of this procedure is to enforce some failures in the cluster and see where the vulnerabilities exist.

##Experiment 1 Pod Failure:##
As a very standard experiment on the cluster is to force kill a pod in a given namespace and see how the cluster reacts in terms of load balancing, and how long will it take until a new pod is created.

##Experiment 1 Results:## 
The experiment ran for a total of 10s while monitoring the status of the pods one pod indeed failed and another one was created almost immedietly after. during the downtime one could still access the website.



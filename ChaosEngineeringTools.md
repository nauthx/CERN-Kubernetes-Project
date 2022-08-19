#Chaos Engineering Tools for Kubernetes

## kube-monkey ##
It is the implementation of Netflix Chaos Monkey for Kubernetes clusters. It randomally deletes pods and can be pre-configured to schedule a random death of a pod.By exposing engineers to failures more frequently it incentivizes them to build resilient services.

## chaoskube ##
Similar to kube-monkey, periodically kills random pods in the kluster. Under default configuration chaos kube is friendly,
when we validate the target cluster it starts its real task and can be configured to have a more agressive interval.

## chaos mesh ##
Standing with the most GitHub stars Chaos Mesh does more than just killing a pod.
- Kills containers in pods

- Network Delays and packet repeats

- Simulates network partition

- Problems with disks and reading/writing

and many more..

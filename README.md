# journal
## Week 1 - Setting up the enviroment and learning the basics of Kubernetes.

First week was about mainly about gaining access and setting up the enviroment for Kubernetes.
I took advantage of the last week of Katacoda which is now discontinued to learn the basics of Kubernetes component and how they intteract with each other in an intteractive browser based experience.

We also went on a couple of tours to explore some of the important CERN sites such as the Data center.

## Week 2 - Team Building and learning the basics on deploying apps in Kubernetes.

After having a meeting with Konstantinos, Rajula and Francisco we have decided to make a plan where my learning goals are targeted as well as the work they want done also is to be targeted.

Initially an issue list was created on a github repo and doing these issues will eventually lead to learn more about Kubernetes and how it's structured.

The first task was:

 Create an Nginx pod serving an index.html that says "Hello world" when you visit the root URL (/).

 I first created a configmap and applied it, inside the configmap the contents of the index.html were also provided which I thought initially as a bit too hard coded.

 Second task was:

  Expose it on your openshift cluster to the external world, so that you can access it from anywhere within the CERN network.

To solve this task I had to do a bit of research on the route/ingress and created a route and inside the configmap for the route, the appropriate port numbers were provided.

Third task was:

 Make sure that we can configure the contents of index.html without changing the pod's image.

 For this I could just type kubectl edit index-html-configmap.yaml and the contents for the index.html were already under 'data' and when they were changed, the contents were also changed.

Fourth task was:

 Observe the nginx logs, which should show every time we hit the URL.

 What was observed that different pods were handling the request, meaning there wasn't just one pod in charge of handling the request but all of them as a form of load balancing!

## Week 3 - Configuring persistent storage on the pods and updating the config map dynamically.

Task Explanation:
Create a persistent storage in the deployment to be seen by all the pods and have a script to be executed
namely every 3 seconds to update the current time on the website by using the date function.
The idea is to mention the path of the persistent storage in the deployment so all the pods created by the deployment 
know where to look for persistent storage.
And inside the persistent storage we provide the script to run so that if a pod dies, the script is carried on by the other pods.


## Week 4 - Falco/GitPod

Summer Student Lectures in the morning until noon

Falco/GitPod Research Phase:

Please refer to FalcoDoc, falcoreview.md, gitpodreview.md.

## Week 5 - Falco

Summer Student Lectures in the morning until noon

In depth research of Falco and Falco rules

## Week 6 - Falco Installation

Summer Student Lectures in the morning until noon

Attempting to install Falco

## Week 7 - Falco Installation/Medical Leave for 3 days

Summer Student Lectures in the morning until noon

Medical leave from Monday until Wednesday

After countlessly trying to install Falco, we came to the conclusion that it is not possible to install falco due to the images we work here with at CERN. and the task is now carried by some other team.


## Week 8 -  Preserving Client IP in Drupal logs

Summer Student/Open Lab Lectures in the morning until noon

Please refer to LogsIssue

## Week 9 - Add Visibility for Intranet/Internet switching

Open Lab Lectures in the morning until noon

Please refer to VisibilityIntranetInternet 

## Week 10 - Stability tests for critical Drupal websites (chaos engineering)

Trying to install Gremlin/Litmus/Chaos Monkey to simulate failures in the clusters. WIP

 




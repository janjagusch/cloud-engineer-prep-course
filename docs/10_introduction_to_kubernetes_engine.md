# Introduction to Kubernetes Engine

## Getting Started with Kubernetes

* Managed service
* Kubernets clusters
* Container orchestration platform
    * Runs Docker containers on a cluster of instances
* Load balancing
* Node pools
* Auto-scaling
* Auto-healing
* Stackdriver monitoring

## Kubernetes Architecture

* Pod
    * Mechanism for encapsulating and running a container
* Deployment
    * Specification of running a certain number of pods with the same container
* Service
    * Wrapper around deployment
    * Associates an IP address to a Pod
    * Provides an endpoint with a stable IP address
* Storage
    * Persistent volumes
        * Exists outside of the pod
    * Persistent volume claim
        * Allows a pod to access a volume

## Deploying a Cluster in Kubernetes Engine using Cloud Shell

* `gcloud container clusters create <name> --zone=<zone> --machine-type=<n1-standard-1> --disk-size=<100>`
* `gcloud container clusters list`

## Deploying Applications in Kubernetes Engine

* Application = Workload
* Running = Deploying
* Kubernetes Engine -> Workload -> Create a deployment

## Quiz

Kubernetes is a ___ orchestration platform.

> container

The smallest deployable unit of computation in Kubernetes is a ___.

> pod

Another term for running an application in Kubernetes is ___.

> deploying

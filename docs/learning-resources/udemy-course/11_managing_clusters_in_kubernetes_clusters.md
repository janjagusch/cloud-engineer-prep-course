# Managing Clusters in Kubernetes Clusters

## Introduction to Kubectl

* Command line utility for running commands on a Kubernetes cluster
* Complements `gcloud container` commands which are used to manage clusters
* Gcloud: Setting up clusters and working with containers
* Kubectl: Manipulate something that exists

## Monitoring Kubernetes

* Stackdriver monitoring -> Resources -> Kubernetes engine
* Kubernetes engine -> Cluster -> Details -> Stackdriver kubernetes engine monitoring (enabled)
* Legacy monitoring should be disabled
* Cluster -> Node (VM) -> Pod -> Container
* Cluster -> Application -> Services

## Viewing the Status of a Kubernetes Cluster

* Kubernetes engine -> Clusters -> Click on cluster
* Node pool (status, version, number of nodes, machine type, image type, autoscaling)
* Node pool = Managed instance group
* Historical values from stackdriver

## Quiz

* What command line utility is used to work with Kubernetes resources within a running cluster?

    > kubectl

* Which GCP service can be used to display performance metrics like CPU utilization and memory utilization?

    > Stackdriver monitoring

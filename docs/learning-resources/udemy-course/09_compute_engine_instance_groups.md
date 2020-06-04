# Group Engine Instance Groups

## Introduction to Managed Instance Groups

* Collection of instances that are managed as a single entity
* Two types
    * Managed instance group
        * MIG
        * Identical VMs
        * Configuration defined in instance template
        * Auto-scaling
        * Auto-healing (health check -> restart)
        * Multi-zone deployment (high availability)
        * Auto-updating
    * Unmanaged instance group
        * Heterogeneous VMs
        * Used behind a load balancer
        * Only recommended for legacy clusters

## Creating a Managed Instance Group

* Compute engine -> Instance groups -> Create instance group
* Instance template -> Create new one:
    * Autosclaing (On)
    * Target CPU utilization (70%)
    * Min number of instances (1)
    * Max number of instances (4)
    * Cooldown period (Before GCP checks the auto-scaling metrics)
    * Health check -> Create health check

## Autoscaling with Managed Instance Groups

* Automatically add or remove instances based on workload
* Set minimum and maximum number of instances
* Based of target utilization
    * Of CPU 
    * HTTP load balancing servicing capacity
    * Stackdriver metrics
* **Cool down period: Time allowed for instances to finish serializing**
* Stabilization period: Time autoscaler uses to calculate recommended number of instances (Avoid thrashing)

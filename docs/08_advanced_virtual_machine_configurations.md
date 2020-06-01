# Advanced Virtual Machine Configurations

## View Virtual Machine Memory

* Compute engine
* You can use filters
* You can use ANDs and ORs to the filter

## Compute Engine Machine Types

* Predefined machine types:
    * Shared core:
        * Run one a single hardware hyperthread
        * Good for non-resource intensive loads
        * Good for short spikes
    * Standard:
        * VCPUs and memory
    * High memory:
        * Useful for memory intensive applications
    * High CPU:
        * Useful for compute intensive applications
    * Mega memory
    * Ultra memory

## Attaching Additional Disks

* Compute engine -> Create instance -> Management, security -> Disks -> Add new disk
* Compute engine -> Disks -> Create disk

## Attaching GPUs

* Create instance -> CPU platform and GPU

## Custom Machine Type

* Create instance -> Machine type -> Custom
* Two slides:
    * Cores
    * Memory

## Creating Snapshots

* Compute engine -> Snapshots -> Create snapshot
* You can add abitrary key-value pairs to the snapshot

## Using Preemptible Virtual Machines

* Preemtible: Can be terminated at any time.
* Saves up to 80% of computing cost.
* Run up to 24 hours before being shut down.
* Good when you can recover from instance failure.
* Create instance -> Networking -> Availability policy -> Preemtibility (On)

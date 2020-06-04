# Starting a Virtual Machine

## Create a Virtual Machine using Cloud Console

* Compute Engine -> VM instances -> Create Instance
    * From scratch
    * From template
    * From marketplace
* From scratch
    * Name
    * Region
    * Zone
    * General purpose/ memory optimized
    * Machine type
    * Boot disk
    * Disk type (SSD) / disk size

## Create a Virtual Machine using Cloud Shell

* `gcloud compute instances create <instance name> --zone=us-west-1-b --machine-type=g1-small --boot-disk-size=16GB`

## Installing the Cloud SDK locally

## Create a Virtual Machine using Cloud SDK

## Accessing a Virtual Machine

* Compute Engine -> Connect (SSH) -> Open in a brower window

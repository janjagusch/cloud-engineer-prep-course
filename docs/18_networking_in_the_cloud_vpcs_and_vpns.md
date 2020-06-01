# Networking in the Cloud: VPCs and VPNs

## Introduction to Networking in the Cloud

* Virtual private cloud
    * Private cloud that you manage within the Google Cloud
    * Global resource
    * VPC network
        * Cloud Router
            * Dynamic routing
            * Allows to connect GCP resources to non-Google networks
* Virtual private network
    * Abstraction to securely connect networks
    * To transfer data securely across the internet
* VPC Peering
    * Sharing resources between VPCs
    * Private communication links
    * With any pair of VPCs
* Shared VPCs
    * Sharing resources between VPCs
    * Available for VPCs of projects within the same organization
* Cloud interconnect
    * Links VPC resources with on-premise data center

## Overview of Virtual Private Clouds

* VPC networks include subnets for regions with distinct, non-overlapping IP address ranges
* VPC networks have default firewall rules in place for basic communnication (ssh, rdp, etc.)
* Routes: How traffic is routed between two resources

## Creating a Virtual Private Cloud

* Create VPC network
    * Name
    * Description
    * Subnetwork creation mode (custom/automatic)
        * Custom
            * Region -> Range
    * Dynamic routing mode (regional/global)

## Overview of Virtual Private Networks

* Hybrid connectivity
* Two types
    * Classic
    * High availability
        * Gateway
        * Tunnels (IPSec)

## Implementing a Virtual Private Network

*

## Cloud and On-Premise Network Integration

*

## Quiz

When creating a VPC and creating default subnets, where are subnets created?

> In all regions

What service allows VPCs to share resources if the VPCs are in different organizations?

> VPC Peering

What two resources must be created to implement a GCP VPN?

> Gateway and a tunnel

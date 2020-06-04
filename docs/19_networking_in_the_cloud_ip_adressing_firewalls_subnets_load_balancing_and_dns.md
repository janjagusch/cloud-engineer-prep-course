# Networking in the Cloud: IP Adressing, Firewalls, Subnets, Load Balancing & DNS

## IP Adressing and CIDR Blocks

* IPv4 (32bit -> Focus in the exam), IPv6 (128bit)
* Adress of device in IP network
* Octet notation (`192.168.2.1`)
* Two parts: Routing prefix (subnet mask), device identifier
* Routing prefix speficied in CIDR notation:
    * 192.168.2.1/24 -> 24 bits used for routing prefix, 8 bits used for device adress
* CIDR: Classless Inter Domain Routing
* Represents block of adresses

## Implementing Firewall Rules

* VPC network -> Firewall rules
* Create firewall rule:
    * Name
    * Description
    * Logs (can get quite large -> pricey)
    * Network
    * Priority (highest priority 0)
    * Direction of traffic (ingress, egress)
    * Allow or deny match
    * Targets
    * Source filter
    * Source IP range
    * Protocols and ports
* Implied firewall rules exist and you cannot delete those
* You can delte the default rules that come when creating a VPC

## Overview of Load Balancing

* Internal vs external
* Global vs regional
* Traffic type (protocol)
* Global load balancers:
    * Workload gets distributed across multiple regions
    * All global load balancers are external
    * Requires premium tier networking
    * Traffic types: HTTP(S), TCP, SSL
* Regional load balancers:
    * Internal: TCP/UPD (for private networks in GCP)
    * External: Network TCP/UDP

## Implementing Load Balancing

* Compute engine -> Create instance group -> Managed instance group
* Network services -> Create load balancer
    * HTTP(S) load balancing
    * Internal or external?
    


## Implementing DNS in GCP

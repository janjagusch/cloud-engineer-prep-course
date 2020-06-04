# Review of GCP Networking Services

## Review of Key Networking Concepts

* Virtual private cloud
    * Global resource
    * Create subnets in regions (in all by default)
    * Resources can communicate using private IP adressing
    * You can share VPCs within organizations
    * You can peer VPCs across organizations
* Virtual private network
    * Links VPC networks to on-premise networks
    * Implemented with IPSec
    * Traffic routed over public internet (encrypted)
    * Up to 3 Gbps
* Cloud interconnect
    * Google networking service
    * Connect directly (> 10 Gbps, < 100 Gbps)
    * Connect through third party (> 50 Mbps, < 10 Gbps)
* Peering
    * Low level network connection
    * Linking networks
    * Traffic routed using Border Gateway Protocol
    * Does not use GCP objects
* Load balancers
    * Global or regional
    * Internal or external
    * Traffic type
        * Global (all external)
            * HTTPS
            * TCP
            * SSL
        * Regional
            * Internal TCP/UPD
            * Network TCP/UPD

## Networking Exam Tips

* Purpose of VPC
* VPC peering vs shared VPC
* Hybrid cloud implementation options
    * VPN
    * Cloud interconnect
    * Peering
* IP adressing and CIDR blocks
* Domain name services
* Load balancing options
* Firewalls
* Routes (BGP)

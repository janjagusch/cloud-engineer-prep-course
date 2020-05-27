# Identity and Access Management

## Introduction to Identity Access Management (IAM) in GCP

* Identity: Representation of a user or entity that has priviledges to perform actions in GCP
* Four types:
    * Google account
        * Represents person (developer, administrator, ...)
        * Email address associated with Google (@gmail.com)
    * Cloud identity or G Suite account
        * Member of a company's G Suite domain
    * Google group
        * Collection of identities
        * Assigning roles to multiple users
    * Service account
        * Not associated with a person but with an application/instance
        * We don't have to use a person identity for machines
* Access control concepts:
    * Resources:
        * VMs, buckets, SQL instances, ...
    * Permission:
        * A holder of a permission can do certain actions on a resource
    * Roles:
        * Predefined
            * Google has created for us
        * Custom
            * Whenever a predefined role doesn't suit our needs
        * Primitive
            * Before IAM existed (not recommended to use)
            * One exception: A small group of people are all responsible across the project
* Policy:
    * Collection of statement which users have access to some resource
    * Roles -> identity
    * Policy -> resource

## Viewing IAM Assignments

* IAM in search box
* Members == identities

## Overview of IAM Roles

* Permission -> Role -> Identity
* Roles in left bar
* Use as many predefined roles as possible

## Creating Custom Roles

* Roles page -> Create role
* Role launch state
    * Alpha, beta: Permissions may change

## Assigning IAM Roles

* IAM main page -> member details

## IAM Best Practices

* Use predefined roles
    * Based on common tasks
    * Minimal set of priviledges
    * Principle of least priviledge
* Define resource structure
    * Attach policies at certain level
* Use groups and service accounts
* Use separate service accounts for separate functions
* Use custom roles sparingly

## Quiz

* A role is a collection of what type of entity?

> Permissions

* What are the two types of IAM roles?

> Custom and predefined

* Where in the cloud console would you go to list all available IAM Roles?

> IAM -> Roles

* What kind of identity is used to grant permissions to a virtual machine to enable it to perform operations in GCP?

> Service account

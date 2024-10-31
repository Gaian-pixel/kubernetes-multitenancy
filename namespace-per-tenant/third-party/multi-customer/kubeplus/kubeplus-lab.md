# Here we are!

## Multi-customer tenancy with [Kubeplus](https://capsule.clastix.io/)

### What is kubeplus?

Capsule is an open source product that implements a multi-tenant and policy-based environment in your Kubernetes cluster. 
It is designed as a micro-services-based ecosystem with the minimalist approach, leveraging only on upstream Kubernetes.

It aggregates multiple namespaces in a lightweight abstraction called Tenant, basically a grouping of Kubernetes Namespaces. Within each tenant, users are free to create their namespaces and share all the assigned resources.

### How capsule work?

![alt text](image.png)

Capsule is a Kubernetes operator (Operators are software extensions to Kubernetes that make use of custom resources to manage applications and their components.) composed by two distinct elements:

* The Capsule Controller: aggregates multiple namespaces in a lightweight abstraction called Tenant
* Capsule Policy Engine: keeps different tenants isolated from each other through the use of network and security policies, resource quota, limit ranges, RBAC, and other tenant-defined policies that are automatically inherited by all namespaces in the tenant.


### The lab scenario

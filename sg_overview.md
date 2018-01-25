---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# About security groups

## What is a security group?
A *security group* is a set of IP filter rules that define how to handle incoming (ingress) and 
outgoing (egress) traffic to both the public and private interfaces of a virtual server instance. The 
rules that you add to a security group are known as *security group rules*.
{:shortdesc}

* You can assign security groups to the public and/or private network interfaces of a single virtual server or multiple virtual server instances.
* You can assign security groups that are provided by IBM or that you create.
* When a security group is applied to a network component of a virtual server instance, all traffic to and from that network component is denied unless explicitly permitted by a security group rule.
* The inbound traffic to a virtual server instance is referred to as ingress traffic.
* The outbound traffic from a virtual server instance is referred to as egress traffic.

Security Groups are implemented on the hypervisor hosting the virtual server.

## Security groups provided by IBM
You can assign any of the following security groups that are provided by IBM® to the network 
interfaces of your virtual server instances:

* *allow_ssh*: This security group defines the IP rules that allow ingress TCP traffic on the SSH port only (22/TCP).
* *allow_http*: This security group defines the IP rules that allow ingress traffic on HTTP port only (80/TCP).
* *allow_https*: This security group defines the IP rules that allow ingress TCP traffic on HTTPS port only (443/TCP).
* *allow_outbound*: This security group defines the IP rules that allow all egress traffic from the server.
* *allow_all*: This security group defines the IP rules that allow all ingress traffic on all ports.

In the following diagram, virtual server instances are 
associated with a set of security groups to restrict network traffic. The arrows represent network traffic flow. The application developer has restricted access to the various infrastructure layers, as follows:

* The application developer can access only the web layer on TCP port 443 (https).
* Only web layer instances can access the application layer instances.
* Only the application layer instances can access the database layer instances. 

![Security group image](images/SecurityGroups.png "Image shows the flow of network traffic with a set of security groups enabled") Figure 1. Security group image



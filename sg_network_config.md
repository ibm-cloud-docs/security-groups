---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Existing network configurations and security groups

A security group augments any existing network configuration. Therefore, a security group cannot span across networks that cannot communicate 
with one another. 
{:shortdesc}

If virtual server instances cannot communicate with one another, adding them to a security group does not change that 
behavior. Gateways must allow the traffic that is defined by the selected security groups.

If your account is enabled for custom private addressing (CPA) as well as security groups, be aware that security groups are scoped to the account level, not the network level. Security groups are defined by IP addresses, not private networks.

Security groups are currently available in the following data centers:

| Data Centers      | 
|:------------------|
| CHE01             |
| DAL12             |
| DAL13             |
| HKG02             |
| HOU02             |
| LON04             |
| MEL01             |
| MEX01             |
| MIL01             |
| MON01             |
| OSL01             |
| SAO01             |
| SJC04             |
| SYD01             |
| SYD04             |
| TOK02             |
| TOR01             |
| WDC06             |
| WDC07             |
{: caption="Table 2. Data centers that support security groups" caption-side="top"} 

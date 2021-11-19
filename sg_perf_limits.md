---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: performance, limits, limitations, rules

subcollection: security-groups


---

{{site.data.keyword.attribute-definition-list}}

# Performance limitations for security groups
{: #performance-limitations-for-security-groups}

Some performance limitations exist for security groups and their associated rules.
{: shortdesc}

| Resource                                                  | Limit                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Security groups per network interface                     | 5                                                   |
| Security groups per account                               | 500                                                 |
| Rules per security group                                  | 50                                                  |
| Remote rules per security group                           | 5                                                   |
| Network interfaces per security group                     | 100                                                 |
{: caption="Table 1. Performance limitations for specific resources" caption-side="bottom"}

A remote rule is one that specifies a security group as the source or destination.
{: note}

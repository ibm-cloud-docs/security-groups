---

copyright:
  years: 2017, 2025
lastupdated: "2025-02-25"

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
{: caption="Performance limitations for specific resources" caption-side="bottom"}

A remote rule is one that specifies a security group as the source or destination. The "Remote rules per security group" resource row illustrates the number of rules that can contain a single security group as a remote group. A maximum of 5 rules can point to a given security group in their remote group field. This is a limit on the number of rules that can reference one security group. Because of performance restrictions, this limit should be set to 0 if you intend to set the "Network Components per security group" limit above 250.
{: note}

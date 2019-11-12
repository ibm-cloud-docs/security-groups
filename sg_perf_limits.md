---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: performance, limits, limitations, rules

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Performance Limitations for Security Groups
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
{: caption="Table 3. Performance limitations for specific resources" caption-side="top"}

A remote rule is one that specifies a security group as the source or destination.
{: note}

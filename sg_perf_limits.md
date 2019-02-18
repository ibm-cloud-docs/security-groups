---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Performance Limitations for Security Groups

Some performance limitations exist for security groups and their associated rules. 
{:shortdesc}

| Resource                                                  | Limit                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Security groups per network interface                     | 5                                                   |
| Security groups per account                               | 500                                                 |
| Rules per security group                                  | 50                                                  |
| Remote rules per security group                           | 5                                                   |
| Network interfaces per security group                     | 100                                                  | 
{: caption="Table 3. Performance limitations for specific resources" caption-side="top"} 

**Note:** A remote rule is one that specifies a security group as the source or destination.
---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Creating a New Rule
Allow incoming requests (SSH & ICMP) and their related (outgoing) traffic flows by performing the following procedure:

1. Select the **Rules** tab in the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window}.2.	Click **Create Rule**.
3.	Specify the rule's Direction, IP Type, Protocol, Port Range, Type, Code and Source when applicable (based on the Protocol selection). 

	Unless you are using another Security Group as the source, leave **Source Type** as "CIDR Block".
	
	![Create a rule](./images/rule_sg.jpg)

	The figure shows **All ICMP** selected as the protocol, which means all ICMP Types and Codes will be allowed. Additionally, the Source field is being left empty, using the default value of `0.0.0.0/0` -- the equivalent to any IP address or subnet.

4.	Click **OK** to finish.


## Next step...
[Assign instances to the Security Group](csg_assign_instances.html) using either the Security Menu or the Device Menu.
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

# 创建和管理定制安全组
在本教程中，您将学习如何创建定制安全组、向其分配实例，以及如何编辑定制安全组。 

![定制安全组](./images/goal.jpg)

## 所需内容
对于此示例，将使用以下对象和项目：

| 资源名称|操作系统|类型| 位置/DC | IP/子网|
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| 不适用/任意| 10.0.0.0/16 |
| allow_icmp |不适用|安全组| 不适用/任意| 0.0.0.0/0 |
| allow_ssh |不适用|安全组| 不适用/任意| 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | 虚拟服务器实例| Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | 虚拟服务器实例|	Dallas 10 Pod 01	| 10.0.2.219 |


请注意，此教程利用 CPA 专用网络/帐户，但是，出于实用目的，安全组在 CPA 帐户和常规帐户中表现相同。子网 10.0.0.0/24 和 10.0.2.0/24 属于同一个 CPA 专用网络，相当于常规帐户的两个或多个 VSI 连接到同一个专用子网/VLAN。


## 要完成的内容

在本教程中，您将学习如何...

任务|描述
------------- | -------------
[创建安全组](csg_create.html) |创建和配置定制安全组，而不是使用 IBM 云平台预定义的一个安全组。
[创建规则](csg_rule.html)  | 创建规则以允许入局请求 (SSH & ICMP) 及其相关的（出局）流量。
[向安全组分配实例](csg_assign_instances.html) | 使用安全菜单或设备菜单向实例分配安全组对象。
[编辑安全组及其规则](csg_edit.html) |修改安全对象及其规则的参数。

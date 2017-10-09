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

# 安全组 API 参考
{: #api-reference} 

SoftLayer&reg; 应用程序编程接口 (API) 这款开发接口使开发人员和系统管理员能够与 SoftLayer 的后端系统进行直接交互。
{:shortdesc}

SoftLayer API (SLAPI) 为客户门户网站中的许多功能部件提供技术支持，这通常意味着，如果交互可以在客户门户网站中进行，就也可以在 API 中运行。因为在 API 中，您可以与 SoftLayer 环境的每个部分进行程序化的交互，所以就可以使用 API 自动执行任务。例如，您可以使用 *SoftLayer_Virtual_Guest/createObject* API 来部署启用了安全组的虚拟服务器实例。

SoftLayer API 是一种远程过程调用系统。每个调用都涉及向 API 端点发送数据以及接收所返回的结构化数据。通过 SLAPI 发送和接收数据时所使用的格式取决于您所选择的 API 实现。 

有关 SoftLayer API、虚拟服务器、安全组 API 的更多信息，请参阅 SoftLayer 开发网络中的以下资源：
* [SoftLayer API 概述 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://sldn.softlayer.com/article/softlayer-api-overview){: new_window} 
* [SoftLayer API 入门 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

您还可以使用 SoftLayer API Python 客户机与安全组进行交互。有关更多信息，请参阅以下链接：
* [SoftLayer API Python 客户机：使用虚拟服务器 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [softlayer_network_securitygroup 的 Python 示例 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}

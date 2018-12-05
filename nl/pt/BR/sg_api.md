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

# Referência de API do Grupo de Segurança
{: #api-reference} 

A Interface de Programação de Aplicações (API) do SoftLayer&reg; é a interface de desenvolvimento que fornece aos desenvolvedores e administradores do sistema a interação direta com o sistema backend do SoftLayer. 
{:shortdesc}

O SoftLayer API (SLAPI) impulsiona muitos dos recursos no Customer Portal, que
geralmente significa que se uma interação é possível no Customer Portal, ela também pode ser executada na API. Como é possível interagir programaticamente
com todas as partes do ambiente SoftLayer dentro da API, é possível usar a API para automatizar tarefas. Por exemplo, é possível usar a
API *SoftLayer_Virtual_Guest/createObject* para implementar uma instância de servidor virtual com um grupo de segurança ativado.

O SoftLayer API é um sistema de Chamada de Procedimento Remoto Cada chamada envolve enviar dados para um terminal de API e receber dados estruturados em retorno. O formato usado para enviar e receber dados com a SLAPI depende de qual implementação da API você escolher. 

Para obter mais informações sobre o SoftLayer API, o servidor virtual e as APIs do grupo de segurança, veja os recursos a seguir no
SoftLayer Development Network:
* [Visão geral do SoftLayer API ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://softlayer.github.io/reference/softlayerapi/){: new_window} 
* [Introdução ao SoftLayer API ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [API *SoftLayer_Virtual_Guest/createObject* ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [API *SoftLayer_Network_SecurityGroup* ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [API *SoftLayer_Virtual_Guest_Network_Component* ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

Também é possível usar o SoftLayer API Python Client para interagir com grupos de segurança. Para obter mais informações, consulte os links a seguir:
* [SoftLayer API Python Client: trabalhando com Virtual Servers ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Exemplos do Python para softlayer_network_securitygroup ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}

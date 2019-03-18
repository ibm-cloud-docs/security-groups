---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Criando e gerenciando um grupo de segurança customizado
{: #creating-and-managing-a-custom-security-group}

Neste tutorial, você aprenderá como criar, designar instâncias para e editar um Grupo de segurança customizada.

![Grupo de segurança customizada](./images/goal.jpg)

## Do que você precisará
Para este exemplo, os objetos e itens a seguir serão usados:

| Nome de Recurso  | Sistema Operacional | Tipo | Local/DC | IP/Sub-rede |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| Não aplicável/Qualquer um | 10.0.0.0/16 |
| allow_icmp | Não aplicável  | Grupo de Segurança | Não aplicável/Qualquer um | 0.0.0.0/0 |
| allow_ssh | Não aplicável | Grupo de Segurança | Não aplicável/Qualquer um | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instância de servidor virtual | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instância de servidor virtual |	Dallas 10 Pod 01	| 10.0.2.219 |


Observe que este tutorial faz uso de uma rede privada/conta de CPA; no entanto, para propósitos práticos, os Grupos de segurança se comportam da mesma forma em contas e contas regulares de CPA. As sub-redes 10.0.0.0/24 e 10.0.2.0/24 pertencem à mesma rede privada de CPA, que seria o equivalente a ter uma conta regular com duas ou mais VSIs conectadas à mesma sub-rede/VLAN privada.


## O que você realizará

Neste tutorial você aprenderá como...

Tarefa  | descrição
------------- | -------------
[Criar um grupo de segurança](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group) | Crie e configure um grupo de segurança customizado, em vez de usar um predefinido pela plataforma de nuvem da IBM©.
[Criar uma regra](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) | Crie uma regra para permitir solicitações recebidas (SSH e ICMP) e seus fluxos de tráfego relacionados (de saída).
[Designar instâncias para o Grupo de segurança](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | Designe objetos do Grupo de segurança para instâncias usando o Menu de segurança ou o Menu de dispositivo.
[Editar um Grupo de Segurança e as suas Regras](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) | Modifique os parâmetros do Objeto de segurança e as suas regras.

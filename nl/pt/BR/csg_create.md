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

# Criando um grupo de segurança
Crie e configure um grupo de segurança customizada:

1. Em seu navegador, abra o [Portal do cliente![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} e efetue login em sua conta.
2.	Selecione a guia **Segurança**.
3. Em **Segurança de rede** selecione **Grupos de segurança**.
4.	Clique em **Criar grupo +**.
5.	Insira um nome para o Grupo de segurança e, opcionalmente, uma descrição.
6. Clique em **Criar Grupo**.

![Criar um grupo de segurança](./images/create_sg.jpg)

Observe que a caixa de seleção **Criar grupo com um padrão…** está desmarcada. Isso significa que nenhuma regra de saída será criada para esse objeto de Grupo de segurança. Como resultado, a menos que outras regras de saída ou objetos de Grupo de segurança sejam criados, somente solicitações recebidas (como SSH e ICMP) e os seus fluxos de tráfego ou respostas relacionados (de saída) serão permitidos.

## Próxima etapa...
[Crie uma regra](csg_rule.html) para permitir solicitações recebidas (SSH e ICMP) e seus fluxos de tráfego relacionados (de saída).  

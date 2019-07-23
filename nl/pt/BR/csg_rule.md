---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, new, rule, ssh, icmp

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Criando uma nova regra
{: #creating-a-new-rule}

Permitir solicitações recebidas (SSH e ICMP) e os seus fluxos de tráfego relacionados (de saída) executando o procedimento a seguir:

1. Selecione a guia **Regras** no [Portal do cliente![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://cloud.ibm.com/classic){: new_window}.
2. Clique em **Criar regra**.
3. Especifique a Direção da regra, o Tipo de IP, o Protocolo, o Intervalo de porta, o Tipo, o Código e a Origem quando aplicável (com base na seleção de Protocolo).

	A menos que você esteja usando outro Grupo de segurança como a origem, deixe **Tipo de origem** como "Bloco do CIDR".

	![Criar uma regra](./images/rule_sg.jpg)

	A figura mostra **Todos os ICMPs** selecionados como o protocolo, o que significa que todos os Tipos de ICMP e Códigos serão permitidos. Além disso, o campo Origem está sendo deixado vazio, usando o valor padrão de `0.0.0.0/0` -- o equivalente a qualquer endereço IP ou sub-rede.

4. Clique em **OK** para concluir.

## Próxima etapa...
{: #next-step-3}

[Designe instâncias para o grupo de segurança](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) usando o Menu de segurança ou o Menu de dispositivo.

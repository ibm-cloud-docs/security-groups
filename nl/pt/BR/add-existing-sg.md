---



copyright:
  years: 2017, 2018
lastupdated: "2018-04-04"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Passo a passo: incluindo um grupo de segurança predefinido durante o pedido
Esse procedimento passo a passo mostra como incluir grupos de segurança existentes ou predefinidos em instâncias durante o processo de pedido.

É possível usar grupos de segurança para decretar um conjunto de regras de filtro de IP que definem como manipular o tráfego de entrada e de saída para as interfaces pública e privada de uma instância de servidor virtual.

![Grupo de segurança customizada](./images/goal2.jpg)

## Do que você precisará
Para este exemplo, os objetos e itens a seguir serão usados:

| Nome de Recurso  | Sistema Operacional | Tipo | Local/DC    | IP/Sub-rede |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | Não aplicável  | Grupo de Segurança | Não aplicável/Qualquer um | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instância de servidor virtual | Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instância de servidor virtual |	Dallas 10 Pod 01	| 10.0.2.219 |

## Pedir um grupo de segurança
Para pedir uma instância de servidor virtual e designar um grupo de segurança, execute o procedimento a seguir:

1. Em seu navegador, abra [Customer Portal ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/) e efetue login em sua conta.
2. Localize a seção **Ordem** e clique em **Dispositivos**.
3. Na página Dispositivos, clique em **Por hora** ou **Mensal** para uma das ofertas de Virtual Server.
4. Na página ordenada Configurar seu servidor em nuvem, selecione um data center que suporte grupos de segurança.
5. Conclua quaisquer outras informações necessárias e clique em **Incluir na ordem**. A página Efetuar check-out é aberta.
6. Confirme as informações a seguir para a VSI: 

	* Endereço
	* Especificações
	* Opções da porta de rede. 

7. Em **Configurar grupos de segurança**, selecione o Grupo de segurança desejado a ser aplicado. As regras associadas a cada Grupo de segurança podem ser exibidas clicando no link **Visualizar regras**. 

	![Grupo de segurança customizada](./images/sgs.jpg)

	É possível selecionar qualquer um dos grupos de segurança predefinidos para aplicar às interfaces privada ou pública no servidor virtual.
	
8. Especifique o nome da instância.
9. Marque os termos do Cloud Service e a caixa de seleção do Contrato de Prestação de Serviços de Terceiro, se aplicável.
10. Por último, clique em **Enviar ordem**.

---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Criando grupos de segurança e regras
{: #creating-security-groups}

É possível criar um grupo de segurança e suas regras associadas e, em seguida, designá-lo às interfaces de uma ou mais instâncias de servidor virtual para ativar um firewall virtual.
{:shortdesc}

## Criando um Grupo de Segurança

Para criar um grupo de segurança, conclua as etapas a seguir:
{:shortdesc}
 
1. Na navegação do [Customer Portal ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/), selecione **Segurança -> Segurança de rede -> Grupos de segurança**.
2. Na página Grupos de segurança, clique em **Criar grupo**.
3. Insira um nome e uma descrição para o grupo de segurança e clique em **Criar grupo** novamente.

**Nota:** "Crie um grupo com uma regra padrão para permitir todo o tráfego de saída." é selecionado por padrão. É possível limpar esse campo para criar o grupo de segurança sem regras. Um grupo de segurança sem regras bloqueia todo o tráfego (de entrada e de saída).

## Criando regras de grupo de segurança

Para criar uma regra de grupo de segurança, conclua as etapas a seguir:
{:shortdesc}

1. Na navegação do [Customer Portal ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/), selecione **Segurança -> Segurança de rede -> Grupos de segurança**.
2. Na página Grupos de segurança, clique em um nome de grupo de segurança para abrir a página Detalhes.
3. Na página de detalhes do Grupo de segurança, insira todas as ações apropriadas (como direção, tipo de IP, protocolo e informações de origem/destino). Quando concluído, clique em **Criar regra**.

**Nota**: para os campos de origem e de destino, é possível especificar o bloco Classless Inter-Domain Routing (CIDR) ou grupo de segurança. 

Um bloco CIDR facilita o roteamento de um bloco de endereços IP.  Se você seleciona CIDR como o tipo, deve-se especificar um intervalo de endereço IP. 

Se você seleciona grupos de segurança como o tipo, então deve-se selecionar de uma lista de grupos de segurança existentes. Essa seleção permite qualquer endereço IP de um dispositivo que esteja conectado ao grupo de segurança selecionado. Se um servidor virtual é configurado para ter múltiplos endereços IP, somente os endereços IPv4 e IPv6 primários são usados por essas regras de grupo de segurança remoto.

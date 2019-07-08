---



copyright:
  years: 2017, 2019
lastupdated: "2019-06-11"

keywords: manage, details, edit, configure

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Gerenciando grupos de segurança
{: #managing-sg}

É possível gerenciar grupos de segurança usando a página Grupos de segurança ou a página Detalhes do dispositivo no portal do cliente de infraestrutura do {{site.data.keyword.cloud}}.
{: shortdesc}

## Gerenciando grupos de segurança na página Grupos de segurança
{: #managing-security-groups-from-security-groups-page}

Para gerenciar grupos de segurança na página Grupos de segurança, conclua as etapas a seguir:

1. Na navegação do [portal do cliente ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/), selecione **Segurança -> Segurança de rede -> Grupos de segurança**.
2. Na seção Grupo de segurança, é possível concluir várias tarefas de gerenciamento.
     * Visualizar uma lista de grupos de segurança.
     * Criar um grupo.
     * Editar informações sobre o grupo.
     * Duplicar um grupo.
     * Exclui um grupo.

## Gerenciando regras de grupo de segurança na página Grupos de segurança
{: #managing-security-group-rules-from-security-groups-page}

Para gerenciar regras de grupo de segurança na página Grupos de segurança, conclua as etapas a seguir:

1. Na navegação do [portal do cliente ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/), selecione **Segurança -> Segurança de rede -> Grupos de segurança**.
2. Clique em um nome de grupo de segurança para abrir a página Detalhes.
3. Na página Detalhes do grupo de segurança, é possível concluir várias tarefas de gerenciamento.
     * Visualizar uma lista de regras que são definidas para o grupo de segurança.
     * Criar novas regras.
     * Editar uma regra.
     * Excluir uma regra.
     * Visualizar as instâncias de servidor virtual e as interfaces associadas que são designadas ao grupo de segurança.

Se você excluir a última regra em um grupo de segurança, nenhum tráfego de entrada ou de saída será permitido por esse grupo de segurança.
{: tip}

## Gerenciando grupos de segurança na página Detalhes do dispositivo
{: #managing-security-groups-from-device-details-page}

Para gerenciar grupos de segurança na página Detalhes do dispositivo, conclua as etapas a seguir:

1. No [portal do cliente ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/), selecione **Dispositivos -> Lista de dispositivos**.
2. Selecione o nome do dispositivo do servidor virtual que você pediu. A página Detalhes do dispositivo é aberta.
3. Na página Detalhes do dispositivo, verifique se você está na guia **Configuração**.
4. Na seção Grupo de segurança, é possível concluir várias tarefas de gerenciamento.
     * Visualizar os grupos de segurança e as regras.
     * Designar grupos de segurança a uma interface de rede de uma instância de servidor virtual.
     * Remover grupos de segurança de uma interface de rede de uma instância de servidor virtual.

     Na primeira vez que você designa um grupo de segurança existente a uma interface de rede (pública ou privada), uma reinicialização é necessária para cada interface.  No entanto, se as interfaces pública e privada são designadas ao grupo de segurança ao mesmo tempo, somente uma reinicialização é necessária.  Após uma reinicialização, as mudanças são aplicadas automaticamente.
     {: important}

     Quando você designa um novo grupo de segurança, ele evita que novas conexões sejam estabelecidas de acordo com as definições de regra de grupo de segurança. No entanto, as conexões do soquete existentes não são finalizadas.

     Se você remover o último grupo de segurança designado a uma instância de servidor virtual, o tráfego do servidor virtual não será mais limitado por grupos de segurança. Um firewall de grupo de segurança não existe mais.
     {: tip}

6. Quando você concluir as mudanças, clique em **Salvar**.

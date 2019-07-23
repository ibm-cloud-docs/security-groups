---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: assign, instance

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# Designando instâncias para o grupo de segurança
{: #assigning-instances-to-the-security-group}

É possível designar objetos de grupo de segurança para instâncias em uma de duas maneiras:

## Usando o menu de Segurança
{: #using-the-security-menu}

1. Na guia **Segurança** no [Portal do cliente![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://cloud.ibm.com/classic){: new_window}, sob **Segurança de rede** selecione **Grupos de segurança**.
2. Clique no ícone ![Ícone mais](./images/more_icon.jpg) do objeto de Grupo de Segurança para o qual você deseja designar instâncias e, em seguida, selecione **Gerenciar instâncias**.
3. Selecione a instância e a interface a serem aplicadas ao Grupo de segurança.

	![Instância do menu de segurança](./images/security_assign.jpg)

	Na figura, o Grupo de segurança "allow_icmp" (criado na [primeira etapa](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group)) é aplicado à interface privada (`10.0.2.219`) de "jpmongevsi4".

	Observe como a contagem de **Instâncias anexadas** aumentou de `0` para `1`.

4. Clique em **Salvar** para aplicar as mudanças.

5. Reinicialize a sua instância.

	Esta é uma etapa única por interface de rede para instâncias não criadas com um grupo de segurança.
  {: note}

## Usando o menu de dispositivos
{: #using-the-devices-menu}

1. Na guia **Dispositivos** no [Portal do cliente![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://cloud.ibm.com/classic){: new_window}, selecione **Lista de dispositivos**.
2. Clique no nome da instância em que você deseja aplicar o objeto de Grupo de segurança.
3. Selecione **Modificar** e marque o objeto de Grupo de segurança que você deseja associar à instância.

	![Instância de menu de dispositivo](./images/device_assign.jpg)

	Esta figura mostra o objeto de Grupo de Segurança "allow_icmp" que está sendo designado para a interface privada da instância jpmongevsi4.
4. Clique em **Salvar** para aplicar as mudanças.

5. Reinicialize a instância.

	Esta é uma etapa única por interface de rede para instâncias não criadas com um grupo de segurança.
  {: note}

## Próxima etapa...
{: #next-step-1}

[Edite o grupo de segurança](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) para modificar os seus parâmetros.  

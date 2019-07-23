---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, configure, configuration, custom

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

# Creación de un Grupo de seguridad
{: #creating-a-security-group}

Cree y configure un grupo de seguridad personalizada:

1. En el navegador, abra el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://cloud.ibm.com/classic){: new_window} e inicie sesión en su cuenta.
2.	Seleccione el separador **Seguridad**.
3. Desde **Seguridad de red**, seleccione **Grupos de seguridad**.
4.	Pulse **Crear grupo +**.
5.	Especifique un nombre para el Grupo de seguridad y, opcionalmente, una descripción.
6. Pulse **Crear grupo**.

![Crear un Grupo de seguridad](./images/create_sg.jpg)

Tenga en cuenta que el recuadro de selección **Crear grupo con un predeterminado…** no está marcado. Esto significa que no se creará ninguna regla saliente para este objeto del Grupo de seguridad. Como resultado, a menos que se creen otras reglas salientes u objetos de Grupo de seguridad, solo se permitirán las solicitudes entrantes (como SSH e ICMP) y sus flujos o respuestas de tráfico relacionadas (salientes).

## Paso siguiente...
{: #next-step-2}

[Cree una regla](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) para permitir las solicitudes entrantes (SSH e ICMP) y sus flujos de tráfico relacionados (salientes).  

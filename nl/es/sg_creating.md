---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Creación de grupos de seguridad y reglas
{: #creating-security-groups}

Puede crear un grupo de seguridad y las reglas asociadas correspondientes y, a continuación, asignarlo a las interfaces de una o varias instancias de servidor virtual para habilitar un cortafuegos virtual.
{:shortdesc}

## Creación de un grupo de seguridad

Para crear un grupo de seguridad, siga estos pasos:
{:shortdesc}
 
1. En la navegación del [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/), seleccione **Seguridad -> Seguridad de red -> Grupos de seguridad**.
2. En la página Grupos de seguridad, pulse **Crear grupo**.
3. Introduzca un nombre y una descripción para el grupo de seguridad y vuelva a pulsar **Crear grupo**.

**Nota:** la opción "Crear grupo con una regla predeterminada que permita todo el tráfico saliente." está seleccionada de forma predeterminada. Puede borrar este campo para crear el grupo de seguridad sin reglas. Un grupo de seguridad sin reglas bloquea todo el tráfico (tanto el entrante como el saliente).

## Creación de reglas de grupos de seguridad

Para crear una regla de grupo de seguridad, siga estos pasos:
{:shortdesc}

1. En la navegación del [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/), seleccione **Seguridad -> Seguridad de red -> Grupos de seguridad**.
2. En la página Grupos de seguridad, pulse un nombre de grupo de seguridad para abrir la página Detalles y seleccione **Crear regla**.
3. En la página Crear regla, introduzca todos los atributos pertinentes (como dirección, tipo de IP, protocolo e información de origen y destino). Cuando haya terminado, pulse **Aceptar**.

**Nota**: La selección de los campos de origen o de destino opcionales restringirán la regla nueva de forma que solo se aplique a tráfico a/desde el origen/destino especificado.  Los campos de origen y de destino pueden especificar un bloque de direccionamiento entre dominios sin clases (CIDR) o un grupo de seguridad. 

Un bloque CIDR facilita el direccionamiento de un bloque de direcciones IP.  Si selecciona como tipo el bloque CIDR, debe especificar un intervalo de direcciones IP. 

Si selecciona como tipo los grupos de seguridad, debe seleccionarlos de una lista de grupos de seguridad existentes. Esta selección permite cualquier dirección IP de dispositivos conectados al grupo de seguridad seleccionado. Si un servidor virtual se ha configurado para tener más de una dirección IP, las reglas de grupos de seguridad remotos solo utilizarán las direcciones IPv4 e IPv6 primarias.

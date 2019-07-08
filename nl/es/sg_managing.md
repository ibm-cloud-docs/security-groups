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

# Gestión de grupos de seguridad
{: #managing-sg}

Puede gestionar grupos de seguridad utilizando la página Grupos de seguridad o la página Detalles del dispositivo en el portal de clientes de la infraestructura de {{site.data.keyword.cloud}}.
{: shortdesc}

## Gestión de grupos de seguridad desde la página Grupos de seguridad
{: #managing-security-groups-from-security-groups-page}

Para gestionar grupos de seguridad desde la página Grupos de seguridad, siga estos pasos:

1. Desde la navegación del [portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/), seleccione **Seguridad -> Seguridad de red -> Grupos de seguridad**.
2. En la sección Grupo de seguridad, puede llevar a cabo varias tareas de gestión.
     * Visualice una lista de grupos de seguridad.
     * Cree un grupo.
     * Edite la información de grupo.
     * Duplique un grupo.
     * Suprima un grupo.

## Gestión de reglas de grupos de seguridad desde la página Grupos de seguridad
{: #managing-security-group-rules-from-security-groups-page}

Para gestionar reglas de grupos de seguridad desde la página Grupos de seguridad, siga estos pasos:

1. Desde la navegación del [portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/), seleccione **Seguridad -> Seguridad de red -> Grupos de seguridad**.
2. Pulse un nombre de grupo de seguridad para abrir la página Detalles.
3. En la sección Detalles del grupo de seguridad, puede llevar a cabo varias tareas de gestión.
     * Visualice una lista de reglas definidas para el grupo de seguridad.
     * Cree reglas.
     * Edite una regla.
     * Suprima una regla.
     * Visualice las instancias de servidor virtual y las interfaces asociadas asignadas al grupo de seguridad.

Si suprime la última regla de un grupo de seguridad, el grupo de seguridad en cuestión no permitirá tráfico entrante ni saliente.
{: tip}

## Gestión de grupos de seguridad desde la página Detalles del dispositivo
{: #managing-security-groups-from-device-details-page}

Para gestionar grupos de seguridad desde la página Detalles del dispositivo, siga estos pasos:

1. Desde el [portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/), seleccione **Dispositivos -> Lista de dispositivos**.
2. Seleccione el nombre del dispositivo del servidor virtual solicitado. Se abrirá la página Detalles del dispositivo.
3. En la página Detalles del dispositivo, asegúrese de estar en el separador **Configuración**.
4. En la sección Grupo de seguridad, puede llevar a cabo varias tareas de gestión.
     * Visualice grupos de seguridad y reglas.
     * Asigne grupos de seguridad a la interfaz de red de una instancia de servidor virtual.
     * Elimine grupos de seguridad de la interfaz de red de una instancia de servidor virtual.

     La primera vez que asigne un grupo de seguridad existente a una interfaz de red (pública o privada), será necesario reiniciar cada interfaz.  Sin embargo, si la interfaz pública y la privada se asignan al grupo de seguridad de forma simultánea, solo se deberá reiniciar una vez.  Tras el reinicio, los cambios se aplican automáticamente.
     {: important}

     Al asignar un nuevo grupo de seguridad, se evita que se establezcan nuevas conexiones según las definiciones de reglas de grupos de seguridad. Sin embargo, las conexiones del socket existentes no se finalizan.

     Si elimina el último grupo de seguridad asignado a una instancia de servidor virtual, el tráfico de servidor virtual dejará de estar limitado por los grupos de seguridad. Ya no existirá ningún cortafuegos de grupo de seguridad.
     {: tip}

6. Cuando haya terminado los cambios, pulse **Guardar**.

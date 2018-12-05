---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Asignación de instancias al Grupo de seguridad
Puede asignar objetos del grupo de seguridad a instancias de una de estas dos formas:

## Utilizando el menú Seguridad

1. Desde el separador **Seguridad** en el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window}, debajo de **Seguridad de red**, seleccione **Grupos de seguridad**.
2. Pulse el icono ![icono Más](./images/more_icon.jpg) del objeto Grupo de seguridad al que desee asignar instancias y, a continuación, seleccione **Gestionar instancias**.
3. Seleccione la instancia y la interfaz a aplicar al Grupo de seguridad.

	![Instancia del menú Seguridad](./images/security_assign.jpg)

	En la figura, el Grupo de seguridad "allow_icmp" (creado en el [primer paso](csg_create.html)) se aplica a la interfaz privada (`10.0.2.219`) de "jpmongevsi4".

	Tenga en cuenta cómo ha aumentado el recuento de **Instancias adjuntas** de `0` a `1`.

4. Pulse **Guardar** para aplicar los cambios.

5. Rearranque la instancia.

	**NOTA:** Este es un paso único por interfaz de red para instancias no creadas con un grupo de seguridad.

## Utilizando el menú Dispositivos

1. Desde el separador **Dispositivos** en el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window}, seleccione **Lista de dispositivos**.
2. Pulse el nombre de instancia donde desea aplicar el objeto Grupo de seguridad.
3. Seleccione **Modificar** y marque el objeto Grupo de seguridad que desee asociar con la instancia.

	![Instancia del menú Dispositivos](./images/device_assign.jpg)

	Esta figura muestra el objeto del Grupo de seguridad "allow_icmp" asignado a la interfaz privada de la instancia jpmongevsi4.
4. Pulse **Guardar** para aplicar los cambios.

5. Rearranque la instancia.

	**NOTA:** Este es un paso único por interfaz de red para instancias no creadas con un grupo de seguridad.

## Paso siguiente...
[Edite el Grupo de seguridad](csg_edit.html) para modificar sus parámetros.  

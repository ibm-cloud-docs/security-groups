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

# Paso a paso: Adición de un Grupo de seguridad predefinido durante la solicitud
Este procedimiento paso a paso le muestra cómo añadir grupos de seguridad existentes o predefinidos a instancias durante el proceso de solicitud.

Puede utilizar los Grupos de seguridad para instaurar un conjunto de reglas de filtro de IP que definen cómo gestionar el tráfico de entrada y el de salida a la interfaz pública y privada de una instancia de servidor virtual.

![Grupo de seguridad personalizado](./images/goal2.jpg)

## Lo que necesitará
Para este ejemplo, se utilizarán los siguientes objetos y elementos:

| Nombre del recurso  | Sistema operativo | Tipo | Ubicación/CD | IP/Subred |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | No aplicable  | Grupo de seguridad | No aplicable/Ninguno | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instancia de servidor virtual | Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instancia de servidor virtual |	Dallas 10 Pod 01	| 10.0.2.219 |

## Solicitar un Grupo de seguridad
Para solicitar una instancia de servidor virtual y asignar un grupo de seguridad, realice el procedimiento siguiente:

1. En el navegador, abra el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/) e inicie sesión en su cuenta.
2. Localice la sección **Pedido** y pulse **Dispositivos**.
3. En la página Dispositivos, pulse **Por hora** o **Mensualmente** para elegir una de las ofertas de servidor virtual.
4. En la página Configurar pedido de servidor de nube, debe seleccionar un centro de datos que dé soporte a grupos de seguridad.
5. Complete la información necesaria y pulse **Añadir a pedido**. Se abrirá la página de pago.
6. Confirme la siguiente información para el VSI: 

	* Ubicación
	* Especificaciones
	* Opciones de puerto de red. 

7. Desde **Configurar grupos de seguridad**, seleccione el Grupo de seguridad deseado que se aplicará. Las reglas asociadas con cada Grupo de seguridad se pueden mostrar pulsando el enlace **Ver reglas**. 

	![Grupo de seguridad personalizado](./images/sgs.jpg)

	Puede seleccionar cualquiera de los grupos de seguridad predefinidos para aplicar a las interfaces públicas o privadas del servidor virtual.
	
8. Especifique el nombre de instancia.
9. Marque el recuadro de selección Términos de servicio de la nube y el Acuerdo de servicio de terceros si es aplicable.
10. Por último, pulse **Enviar pedido**.

---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Referencia de API de grupo de seguridad
{: #api-reference} 

La API de SoftLayer&reg; es la interfaz de desarrollo que permite a los desarrolladores y administradores del sistema interactuar directamente con el sistema de fondo de SoftLayer. 
{:shortdesc}

La API de SoftLayer (SLAPI) ofrece muchas de las características del Portal de clientes, lo cual significa que normalmente si una interacción es posible en Portal de clientes, también lo es en la API. Puesto que se puede interactuar mediante programación con todos los componentes del entorno de SoftLayer dentro de la API, es posible utilizar la API para automatizar tareas. Por ejemplo, puede utilizar la API *SoftLayer_Virtual_Guest/createObject* para desplegar una instancia de servidor virtual con un grupo de seguridad habilitado.

La API de SoftLayer es un sistema de llamada a procedimiento remoto. Cada llamada implica el envío de datos a un punto final de API y la recepción de datos estructurados. El formato utilizado para enviar y recibir datos con la SLAPI depende de la implementación de la API que se elija. 

Para obtener más información sobre la API SoftLayer, el servidor virtual y las API de los grupos de seguridad, consulte los siguientes recursos en la red de despliegue de SoftLayer:
* [Visión general de la API de SoftLayer ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://softlayer.github.io/reference/softlayerapi/){: new_window} 
* [Iniciación a la API de SoftLayer ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

También puede utilizar el cliente Python de la API SoftLayer para interactuar con los grupos de seguridad. Para obtener más información, consulte los siguientes enlaces:
* [Cliente Python de la API de Softlayer: Cómo trabajar con servidores virtuales ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Ejemplos de Python para softlayer_network_securitygroup ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}

---



copyright:
  years: 2017, 2018
lastupdated: "2018-04-04"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Iniciación a los grupos de seguridad

Puede utilizar los Grupos de seguridad para instaurar un conjunto de reglas de filtro de IP que definen cómo gestionar el tráfico de entrada y el de salida a la interfaz pública y privada de una instancia de servidor virtual.
{:shortdesc}

Para empezar, solicite una instancia de servidor virtual (VSI) y asigne un grupo de seguridad.
 
1. En el navegador, abra el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/) e inicie sesión en su cuenta.
2. Localice la sección **Pedido** y pulse **Dispositivos**.
3. En la página Dispositivos, pulse **Por hora** o **Mensualmente** para elegir una de las ofertas de servidor virtual.
4. En la página **Configurar pedido de servidor de nube**, debe seleccionar un centro de datos que dé soporte a grupos de seguridad.
5. Complete la información necesaria y pulse **Añadir a pedido**. Se abrirá la página de pago.
6. Complete la información de **Configurar grupos de seguridad**.
7. Puede seleccionar cualquiera de los grupos de seguridad predefinidos para aplicar a las interfaces públicas o privadas del servidor virtual.
8. Por último, pulse **Enviar pedido**.

## Casos prácticos y soluciones
Las secciones siguientes describen algunos casos de ejemplo difíciles de seguridad de red con los que puede encontrarse que pueden solucionarse utilizando Grupos de seguridad.

### Seguridad desde el inicio
**Caso de ejemplo de seguridad:** Los clientes desean proteger su servidor virtual siempre que se proporcione. Desean control completo sobre el tráfico que pasa a través del servidor desde el punto en que se proporcionó.

**Solución:** Utilice Grupos de seguridad en el momento de solicitar el servidor virtual. De esta forma, el servidor estará protegido desde el momento en que se proporcione.

### Cortafuegos de nivel de instancia rentable
**Caso de ejemplo de seguridad:** Los clientes desean tener control granular sobre el tráfico en un nivel de instancia (aparte del cortafuegos a nivel de red) pero, al mismo tiempo, los costes de un cortafuegos de hardware compartido (que es la oferta de cortafuegos de varios arrendatarios de otro nivel de instancias de IBM) pueden añadirse rápidamente si el cliente necesita proteger varios servidores en distintos centros de datos.

**Solución:** No hay cargo extra para utilizar la característica Grupos de seguridad. Utilice los Grupos de seguridad para todos los servidores virtuales que necesitan protección en cualquiera de nuestros centros de datos globales.

### Cortafuegos globalmente escalable y fácilmente gestionable
**Caso de ejemplo de seguridad:** Los clientes desean evitar configurar reglas de cortafuegos en cada servidor por separado. En su lugar, desean una solución de cortafuegos fácilmente gestionable que abarque servidores en distintos centros de datos globales.

**Solución:** Defina `N` Grupos de seguridad para `N` tipos distintos de servidores en la carga de trabajo de nube. Gestione todas las reglas para un grupo de seguridad en un lugar. Gestione las asociaciones del grupo de seguridad de forma apropiada con los servidores virtuales.

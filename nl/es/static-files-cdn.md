---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Acelerar la entrega de archivos estáticos utilizando el Almacenamiento de objetos y CDN
Permita las solicitudes entrantes (SSH e ICMP) y sus flujos de tráfico relacionados (salientes) realizando el procedimiento siguiente:

1. Seleccione el separador **Reglas** en el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window}.
2.	Pulse **Crear regla**.
3.	Especifique la Dirección, el Tipo de IP, el Protocolo, el Rango de puertos, el Tipo, el Código y el Origen de la regla cuando sea aplicable (en función de la selección del Protocolo).

	A menos que esté utilizando otro Grupo de seguridad que el origen, deje **Tipo de origen** como "Bloque de CIDR".

	![Crear una regla](rule_sg.jpg)

	La figura muestra **Todos los ICMP** seleccionados como el protocolo, lo que significa que se permitirán todos los Tipos y Códigos de ICMP. Adicionalmente, el campo Origen se está dejando vacío, utilizando el valor predeterminado de `0.0.0.0/0` -- el equivalente a cualquier dirección IP o subred.

4.	Pulse en **Aceptar** para finalizar.

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

# Creación y gestión de un grupo de seguridad personalizada
En esta guía de aprendizaje aprenderá cómo crear, asignar instancias a y editar un Grupo de seguridad personalizado. 

![Grupo de seguridad personalizado](./images/goal.jpg)

## Lo que necesitará
Para este ejemplo, se utilizarán los siguientes objetos y elementos:

| Nombre del recurso  | Sistema operativo | Tipo | Ubicación/CD | IP/Subred |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| No aplicable/Ninguno | 10.0.0.0/16 |
| allow_icmp | No aplicable  | Grupo de seguridad | No aplicable/Ninguno | 0.0.0.0/0 |
| allow_ssh | No aplicable | Grupo de seguridad | No aplicable/Ninguno | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instancia de servidor virtual | Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instancia de servidor virtual |	Dallas 10 Pod 01	| 10.0.2.219 |


Tenga en cuenta que esta guía de aprendizaje utiliza una red/cuenta privada de CPA; sin embargo, por razones prácticas, los Grupos de seguridad se comportan de la misma forma en las cuentas de CPA y en las cuentas normales. Las subredes 10.0.0.0/24 y 10.0.2.0/24 pertenecen a la misma red privada de CPA, que sería el equivalente de tener una cuenta normal con dos o más VSI conectados a la misma subred/VLAN privada.


## Qué conseguirá

En esta guía de aprendizaje aprenderá a...

Tarea  | Descripción
------------- | -------------
[Crear un Grupo de seguridad](csg_create.html) | Crear y configurar un grupo de seguridad personalizada, al contrario que utilizar uno predefinido mediante la plataforma de IBM Cloud. 
[Crear una regla](csg_rule.html)  | Crear una regla para permitir las solicitudes entrantes (SSH e ICMP) y sus flujos de tráfico relacionados (salientes). 
[Asignar instancias al Grupo de seguridad](csg_assign_instances.html) | Asignar objetos de Grupo de seguridad a instancias utilizando el menú Seguridad o el menú Dispositivos.
[Editar un Grupo de seguridad y sus Reglas](csg_edit.html) | Modificar los parámetros del Objeto de seguridad y de sus reglas.
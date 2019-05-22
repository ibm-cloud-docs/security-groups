---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introdução aos grupos de segurança
{: #getting-started}

É possível usar grupos de segurança para decretar um conjunto de regras de filtro de IP que definem como manipular o tráfego de entrada e de saída para as interfaces pública e privada de uma instância de servidor virtual.
{:shortdesc}

Para iniciar, solicite uma instância de servidor virtual (VSI) e designe um grupo de segurança.

1. Em seu navegador, abra [Customer Portal ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/) e efetue login em sua conta.
2. Localize a seção **Ordem** e clique em **Dispositivos**.
3. Na página Dispositivos, clique em **Por hora** ou **Mensal** para uma das ofertas de Virtual Server.
4. Na página ordenada **Configurar seu servidor em nuvem**, selecione um data center que suporte grupos de segurança.
5. Conclua quaisquer outras informações necessárias e clique em **Incluir na ordem**. A página Efetuar check-out é aberta.
6. Conclua as informações de **Configurar grupos de segurança**.
7. É possível selecionar qualquer um dos grupos de segurança predefinidos para aplicar às interfaces privada ou pública no servidor virtual.
8. Por último, clique em **Enviar ordem**.

## Casos de uso e soluções
As seções a seguir descrevem alguns cenários de segurança de rede difíceis que é possível encontrar e que podem ser aliviados usando Grupos de segurança.

### Segurança desde o início
**Cenário de segurança:** os clientes desejam proteger o seu servidor virtual assim que ele for provisionado. Eles desejam controle total sobre o tráfego que passa pelo servidor desde o ponto em que ele foi provisionado.

**Solução:** use os Grupos de segurança no momento do pedido do servidor virtual. Dessa forma, o seu servidor será protegido desde o momento em que for provisionado.

### Firewall de nível de instância com custo eficiente
**Cenário de segurança:** os clientes querem ter controle granular sobre o tráfego a um nível de instância (diferente do firewall de nível de rede), mas, ao mesmo tempo, os custos de um firewall de hardware compartilhado (que é outro nível de instância fornecido pela IBM© de uma oferta de firewall de vários locatários) podem aumentar rapidamente caso o cliente precise proteger vários servidores em diferentes data centers.

**Solução:** não há encargo extra para usar o recurso de Grupos de segurança. Use Grupos de segurança para todos os servidores virtuais que precisam de proteção em qualquer um de nossos data centers globais.

### Firewall globalmente escalável e facilmente gerenciável
**Cenário de segurança:** os clientes querem evitar a configuração de regras de firewall em cada servidor separadamente. Em vez disso, eles querem uma solução de firewall facilmente gerenciável que abranja servidores em diferentes data centers globais.

**Solução:** defina `N` Grupos de segurança para `N` tipos de servidores diferentes em sua carga de trabalho de nuvem. Gerencie todas as regras para um grupo de segurança em um local. Gerencie as associações de grupo de segurança adequadamente com os servidores virtuais.

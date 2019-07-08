---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: security, guidelines, rules

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Diretrizes dos grupos de segurança
{: #security-groups-guidelines}

Considere as diretrizes a seguir ao trabalhar com grupos de segurança:

## Rules
{: #rules-1}

* Cada grupo de segurança define diferentes conjuntos de regras de rede que definem o tráfego de entrada e de saída para uma instância de servidor virtual. É possível especificar regras para ambos, IPv4 e IPv6.
* Quando um novo grupo de segurança é criado usando a interface do Customer Portal, o comportamento padrão é criar uma única regra que permita todo o tráfego de saída da instância de servidor virtual. Deve-se limpar a caixa de seleção "Criar grupo com uma regra padrão para permitir todo o tráfego de saída" para criar o grupo de segurança sem regras. Um grupo de segurança sem regras bloqueia todo o tráfego (de entrada e de saída).
* Para permitir o tráfego de entrada, tráfego de saída ou ambos, deve-se incluir pelo menos um grupo de segurança que inclua regras de grupo de segurança que permitam tráfego.
* As regras de grupo de segurança podem ser somente permissivas. O tráfego é bloqueado por padrão.
* Os usuários com o privilégio Gerenciar grupos de segurança podem incluir, editar ou excluir regras em um grupo de segurança.
* As mudanças nas regras de grupo de segurança são aplicadas automaticamente e podem ser modificadas a qualquer momento.
* A ordem das regras em um grupo de segurança não importa. A prioridade sempre cai na regra menos restritiva.
* As regras são stateful. Conexões estabelecidas antes de uma mudança de grupo de segurança não serão alteradas. Novas conexões obedecerão às regras que existirem no momento em que a conectividade for estabelecida.
* Os grupos de segurança não substituem os firewalls do sistema operacional no servidor virtual. Mesmo se existir, no sistema operacional, um firewall mais restritivo do que aquele que é aplicado pelo grupo de segurança, as regras do sistema operacional ainda serão cumpridas.
* Se o seu servidor virtual precisar de acesso a serviços internos, como um servidor de atualização, armazenamento conectado à rede (NAS) ou monitoramento avançado, assegure-se de que as regras de grupo de segurança acomodem o tráfego para esses serviços internos. Para obter mais informações, consulte [Quais intervalos de IP permitir por meio do firewall](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-ibm-cloud-ip-ranges).

## Interfaces
{: #interfaces-1}

* Um grupo de segurança pode ser aplicado a uma rede privada, uma rede pública ou a ambos os tipos de interface de rede.
* É possível anexar um ou mais grupos de segurança à lista de grupos de segurança que são designados a uma interface de rede. As regras de grupo de segurança de cada grupo de segurança se aplicam às instâncias de servidor virtual associado.
* Na primeira vez que você designa um grupo de segurança existente a uma interface de rede (pública ou privada), uma reinicialização é necessária para cada interface.  No entanto, se as interfaces pública e privada são designadas ao grupo de segurança ao mesmo tempo, somente uma reinicialização é necessária.  Após uma reinicialização, as mudanças são aplicadas automaticamente.

## Acessar
{: #access-1}

* Todos os usuários em uma conta podem ler, anexar e remover grupos de segurança nas instâncias de servidor virtual às quais eles têm acesso. Somente usuários com o privilégio para Gerenciar grupos de segurança em Permissões de rede podem criar, atualizar ou excluir grupos de segurança
* Não é possível designar grupos de segurança a servidores bare metal.

## Exclusão
{: #deletion-1}

* Não é possível excluir um grupo de segurança que está designado a uma ou mais instâncias de servidor virtual em execução.
* Não é possível excluir um grupo de segurança que outro grupo de segurança está referenciando em uma de suas regras.

---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurações de rede e grupos de segurança existentes

Um grupo de segurança aumenta qualquer configuração de rede existente. Portanto, um grupo de segurança não pode abranger redes que não podem se comunicar
entre si. 
{:shortdesc}

Se as instâncias de servidor virtual não podem se comunicar entre si, incluí-las em um grupo de segurança não muda esse
comportamento. Os gateways devem permitir o tráfego definido pelos grupos de segurança selecionados.

Se a sua conta está ativada para o custom private addressing (CPA), bem como grupos de segurança, esteja ciente de que os grupos de segurança têm o escopo definido para o nível de conta, não no nível de rede. Os grupos de segurança são definidos por endereços IP, não redes privadas.

Os grupos de segurança estão disponíveis atualmente nos data centers a seguir:

| Data Centers      | 
|:------------------|
| AMS01             |
| AMS03             |
| CHE01             |
| DAL01             |
| DAL05             |
| DAL06             |
| DAL09             |
| DAL10             |
| DAL12             |
| DAL13             |
| FRA02             |
| FRA04             |
| FRA05             |
| HKG02             |
| HOU02             |
| LON02             |
| LON04             |
| LON06             |
| MEL01             |
| MEX01             |
| MIL01             |
| MON01             |
| OSL01             |
| PAR01             |
| SAO01             |
| SEA01             |
| SEO01             |
| SJC01             |
| SJC03             |
| SJC04             |
| SNG01             |
| SYD01             |
| SYD04             |
| TOK02             |
| TOR01             |
| WDC01             |
| WDC04             |
| WDC06             |
| WDC07             |
{: caption="Tabela 2. Data centers que suportam grupos de segurança" caption-side="top"} 

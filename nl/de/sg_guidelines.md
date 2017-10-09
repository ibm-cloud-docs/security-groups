---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Richtlinien für Sicherheitsgruppen
Beachten Sie beim Arbeiten mit Sicherheitsgruppen die folgenden Richtlinien:

## Regeln

* Jede Sicherheitsgruppe definiert unterschiedliche Gruppen von Netzregeln, die den eingehenden und abgehenden Datenverkehr für eine virtuelle Serverinstanz definieren. Sie können Regeln sowohl für IPv4 als auch für IPv6 angeben.
* Das Standardverhalten beim Erstellen einer neuen Sicherheitsgruppe mithilfe der Schnittstelle 'Kundenportal' sieht vor, dass eine einzelne Regel erstellt wird, die den gesamten abgehenden Datenverkehr von der virtuellen Serverinstanz zulässt. Sie müssen das Kontrollkästchen abwählen, mit dem eine Gruppe mit einer Standardregel erstellt wird, die sämtlichen abgehenden Datenverkehr zulässt. Dann wird die Sicherheitsgruppe ohne Regeln erstellt. Eine Sicherheitsgruppe ohne Regeln blockiert sämtlichen Datenverkehr (sowohl eingehenden als auch abgehenden).
* Um eingehenden Datenverkehr, abgehenden Datenverkehr oder beide Arten von Datenverkehr zuzulassen, müssen Sie mindestens eine Sicherheitsgruppe hinzufügen, die Sicherheitsgruppenregeln enthält, durch die Datenverkehr zulässig ist. 
* Sicherheitsgruppenregeln können nur tolerant sein. Standardmäßig wird Datenverkehr geblockt.
* Benutzer mit der Berechtigung zum Verwalten von Sicherheitsgruppen können Regeln in einer Sicherheitsgruppe hinzufügen, bearbeiten oder löschen. 
* Änderungen an Sicherheitsgruppenregeln werden automatisch angewendet und können jederzeit geändert werden.
* Die Reihenfolge der Regeln in einer Sicherheitsgruppe spielt keine Rolle. Vorrang hat jeweils die am wenigsten einschränkende Regel.
* Sicherheitsgruppen setzen auf dem virtuellen Server keine Firewalls des Betriebssystems außer Kraft. Wenn unter dem Betriebssystem eine Firewall vorhanden ist, die einschränkender ist als die Vorgaben der Sicherheitsgruppen, werden die Betriebssystemregeln dennoch umgesetzt.
* Wenn Ihr virtueller Server Zugriff auf interne Services wie beispielsweise auf einen Aktualisierungsserver, Network Attached Storage (NAS) oder erweiterte Überwachung benötigt, müssen Sie sicherstellen, dass die Sicherheitsgruppenregeln den für diese internen Services erforderlichen Datenverkehr ermöglichen. Weitere Informationen finden Sie unter [Welche IP-Bereiche darf die Firewall zulassen? ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://knowledgelayer.softlayer.com/faqs/6#154) und [Unter Linux auf Blockspeicher zugreifen ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://knowledgelayer.softlayer.com/procedure/block-storage-linux).

## Schnittstellen

* Eine Sicherheitsgruppe kann auf ein privates Netz, ein öffentliches Netz oder auf beide Netzschnittstellentypen angewendet werden.
* Sie können an die Liste mit Sicherheitsgruppen, die einer Netzschnittstelle zugeordnet sind, mindestens eine Sicherheitsgruppe anhängen. Die Sicherheitsgruppenregeln der einzelnen Sicherheitsgruppen gelten für die zugeordneten virtuellen Serverinstanzen. 
* Beim erstmaligen Zuordnen einer vorhandenen Sicherheitsgruppe zu einer Netzschnittstelle (öffentlich oder privat) ist für jede der Schnittstellen ein Neustart erforderlich. Wenn die öffentlichen und privaten Schnittstellen der Sicherheitsgruppe jedoch gleichzeitig zugeordnet wurden, ist nur ein einziger Neustart erforderlich. Nach einem Neustart werden Änderungen automatisch angewendet.

## Zugriff
 
* Innerhalb eines Kontos können alle Benutzer auf den virtuellen Serverinstanzen, für die sie Zugriff haben, Sicherheitsgruppen lesen, anhängen und abhängen. Sicherheitsgruppen erstellen, aktualisieren und löschen können nur Benutzer, die in den Netzberechtigungen (Network Permissions) die Berechtigung zum Verwalten von Sicherheitsgruppen haben.
* Bare-Metal-Servern können Sie keine Sicherheitsgruppen zuordnen.

## Löschvorgänge

* Sie können eine Sicherheitsgruppe, die mindestens einer aktiven virtuellen Serverinstanz zugeordnet ist, nicht löschen.
* Sie können eine Sicherheitsgruppe, auf die eine andere Sicherheitsgruppe in mindestens einer ihrer Regeln verweist, nicht löschen. 

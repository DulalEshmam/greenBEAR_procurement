# greenBEAR Procurement (`greenbear_procurement`)

greenBear_Procurement ist ein importierbares Odoo-Datenmodul, das den Odoo-Einkauf um einen vorgelagerten Beschaffungsvorgang, eine Vorab-Mittelbindung und eine eigene Budgetübersicht ergänzt. Freigegebene Bedarfe werden demnach bereits vor der Bestellbestätigung als gebundene Mittel berücksichtigt.
Der Pilot weist die zentrale Prozess- und Budgetlogik im vereinfachten Beschaffungsfall nach. Er ist nicht als produktionsreife Lösung freigegeben


## Funktionen
- Beschaffungsvorgang mit automatischer Referenz GB-BES-JJJJ-NNNN, Antragsteller, verantwortlicher Person, Betrag, Begründung und fünf Budgetdimensionen
- Statusgesteuerter Workflow über rollenbeschränkte Aktionen (Statusfeld schreibgeschützt)
- Vorab-Mittelbindung (GB-VMB-JJJJ-NNNN): wird beim Einreichen vorgemerkt, bei Freigabe aktiv und bei Bestellbestätigung an die Bestellung übergeben – ohne Doppelzählung
- Budgetübersicht je Kombination aus Saison, Modul/Bereich, Baugruppe/Komponente, Unterkategorie und Finanzierungsquelle
- Bestellintegration: Verknüpfung von Angebotsanfrage/Bestellung (purchase.order) mit dem Vorgang; gebuchte Lieferantenrechnungen ersetzen den Bestellbetrag
- Überschreitungswarnung: Warnhinweis am Vorgang und einmalige To-do-Aktivität für Finance



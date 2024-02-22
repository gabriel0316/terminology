> **For the english version please click [here](index_en.html).**

### Willkommen auf dem neuen österreichischen e-Health Terminologiebrowser!

Der Terminologieserver bietet den Stakeholdern des österreichischen Gesundheitswesens die Möglichkeit Terminologien über das Internet bereit zu stellen und ermöglicht Terminologie-Recherche sowie Terminologie-Download in verschiedenen Formaten. Ziel ist es, dass die IT-Systeme, die untereinander in einer Datenaustausch-Beziehung stehen, dieselben Terminologien zur selben Zeit verwenden können. Codesysteme und Value Sets werden gemeinsam mit den dazugehörigen historischen Versionen in standardisierten Formaten und einheitlichen Metadaten leicht zugänglich bereitgestellt.

### Technologiebasis

Technologisch basiert das österreichische e-Health Terminologie-System auf TerminoloGit. Siehe dazu die [technische Dokumentation](technical_documentation_de.html).

### FAQ

Die wichtigsten Fragen und Antworten zum Terminologieserver sind hier zusammengefasst.

#### Wo finde ich Codelisten/Codesysteme und Value Sets, die ich bisher verwendet habe?
Über [Table of Contents](https://termgit.elga.gv.at/toc.html) bzw. [Artifact Summary](https://termgit.elga.gv.at/artifacts.html) können die Terminologien abgerufen werden. Zur einfacheren Lesbarkeit wurden lediglich die Postfixes (z.B. "_CS" oder "_VS") entfernt. Sobald man auf eine Terminologie klickt, werden in der Summary die Details, wie zum Beispiel, ob es sich um ein Codesystem oder Value Set handelt, angezeigt.

Table of Contents listet alle Terminologien alphabetisch. Unter der Artifact Summary werden alle Terminologien nach Codesystemen bzw. Value Sets gruppiert.

Eine erweiterte Suche wird noch implementiert.

#### Welche Downloadformate gibt es? Wie entsprechen die neuen Formate jenen des alten Terminologieservers?

Aktuell werden folgende Downloadformate unter dem Reiter `Download` der jeweiligen Terminologie angeboten:

| *neuer* Terminologieserver | *alter* Terminologieserver | Hinweis |
| ----------- | ----------- | ----------- |
| FHIR R4 xml `.4.fhir.xml` | keine Entsprechung       | |
| FHIR R4 json `.4.fhir.json`   | keine Entsprechung        | |
| fsh v1 `.1.fsh`   | keine Entsprechung        | |
| fsh v2 `.2.fsh`   | keine Entsprechung        | |
| ClaML v2 `.2.claml.xml`   | ClaML        | |
| ClaML v3 `.3.claml.xml`   | keine Entsprechung        | |
| propCSV v1 `.1.propcsv.csv`   | keine Entsprechung        | |
| SVSextELGA v1 `.1.svsextelga.xml`   | SVS        | **Achtung! DEPRECATED!**<br/>Dieses Format kann technisch gesehen nicht alle Informationen enthalten,<br/>die in den anderen Formaten verfügbar sind.<br/>Dieses Format ist nur für Legacy-Zwecke verfügbar. |
| SVSextELGA v2 `.2.svsextelga.xml`   | keine Entsprechung        | **Achtung! DEPRECATED!**<br/>Dieses Format kann technisch gesehen nicht alle Informationen enthalten,<br/>die in den anderen Formaten verfügbar sind.<br/>Dieses Format ist nur für Legacy-Zwecke verfügbar.<br/> Es sind hier jedoch alle Eigenschaften zu Konzepten verfügbar. |
| outdatedCSV v1 `.1.outdatedcsv.csv`   | CSV nach TermPub Standard | **Achtung! DEPRECATED!**<br/>Dieses Format kann technisch gesehen nicht alle Informationen enthalten,<br/>die in den anderen <br/>Formaten verfügbar sind.<br/>Dieses Format ist nur für Legacy-Zwecke verfügbar. |
| outdatedCSV v2 `.2.outdatedcsv.csv`   | CSV wie es <br/>von TermPub geliefert wird <br/>(an TermPub Standard angelehnt) | **Achtung! DEPRECATED!**<br/>Dieses Format kann technisch gesehen nicht alle Informationen enthalten,<br/>die in den anderen Formaten verfügbar sind.<br/>Dieses Format ist nur für Legacy-Zwecke verfügbar.<br/> Es sind hier jedoch alle Eigenschaften zu Konzepten verfügbar. |

Eine detailliertere Beschreibung der einzelnen Downloadformate kann [in der technischen Dokumentation](file_formats_de.html) abgerufen werden.

#### Wie erkenne ich, welche Terminologie die aktuelle ist?

Die Terminologien, die über [Table of Contents](https://termgit.elga.gv.at/toc.html) bzw. [Artifact Summary](https://termgit.elga.gv.at/artifacts.html) angezeigt und aufgerufen werden können, stellen immer die aktuellsten Versionen dar.

Table of Contents listet alle Terminologien alphabetisch. Unter der Artifact Summary werden alle Terminologien nach Codesystemen bzw. Value Sets gruppiert.

#### Wo finde ich alte Versionen?

Mit dem neuen Terminologieserver können für jede Terminologie unter dem Reiter `Previous Versions` alle publizierten Versionen abgerufen werden. Bei der Darstellung von alten Versionen wird jeweils ein Warnhinweis angezeigt, dass es sich um eine alte Version handelt. Dieser Hinweis beinhaltet auch einen Link auf die aktuelle Terminologieversion.

Der alte Terminologieserver wurde bis Oktober 2022 betrieben. Falls spezielle alte Versionen von Terminologien (vor 2022) gesucht werden, können diese beim CDA Team [cda@elga.gv.at](mailto:cda@elga.gv.at) angefragt werden.

#### Wie kann ich von Updates benachrichtigt werden?

Siehe [automatischer Import von Terminologien](use_cases_de.html#automatischer-import-von-terminologien) bzw. [manueller Import von Terminologien](use_cases_de.html#manueller-import-von-terminologien).

#### Wie kann man Änderungen vorschlagen oder Fehler melden?

Bitte, beachten Sie die [Support-Seite](support_de.html).

### Die ELGA- & österreichische eHealth-Terminologien

In ELGA und den österreichischen eHealth-Systemen wird eine Vielzahl unterschiedlicher Terminologien mit unterschiedlicher Struktur von verschiedenen internationalen, nationalen und lokalen Quellen verwendet. Über TerminoloGit werden diese in eine möglichst einheitliche Form gebracht und hier sichtbar gemacht.

Alle Terminologien und deren Änderungen sind am Terminologieserver zentral abrufbar und werden zusätzlich mit Updatemeldungen unter https://confluence.elga.gv.at/display/SCCTERM bekannt gemacht. Prüfungen auf geänderte Terminologien sollten mindestens **wöchentlich** erfolgen.

Alle mit dieser Dokumentation nicht beantwortbaren Fragen zu ELGA- und österreichischen e-Health-relevanten Terminologien können an [cda@elga.gv.at](mailto:cda@elga.gv.at) gemeldet werden. Von dieser Adresse aus wird die Bearbeitung zentral koordiniert.

Bei Terminologien wird zwischen Codesytemen und Value Sets unterschieden.

#### Codesysteme

Unter einem Codesystem ist die Sammlung von Codes zu verstehen, wie auch deren Metadaten und den Metadaten des Codesystems selbst. Codesysteme können auch eine Ontologie, Tabelle oder einfache Aufzählung sein. [LOINC](https://loinc.org/), [SNOMED CT](https://www.snomed.org/) und [HL7® CodeSystems](https://www.hl7.org/fhir/codesystem-gender-identity.html) sind Beispiele solcher Codesysteme.

Die Aktualisierung von Codesystemen und deren Zeitpunkt oder Häufigkeit liegt in der Verantwortung der Ersteller und damit meist außerhalb des Einflussbereiches von ELGA. Codesysteme können nur dann außerhalb der Verantwortung der Ersteller korrigiert werden, wenn ein technisches Problem vorliegt.

Ein Codesystem wird nicht nur durch einen eindeutigen Namen, sondern auch durch eine OID eindeutig identifiziert. Die Bedeutung eines Codes kann nur gemeinsam mit dem Namen/URI oder der OID des Codesystems entschlüsselt werden.

Ein Grundsatz der Terminologie-Entwicklung ist, dass Codes nicht gelöscht und auch die Bedeutung eines Codes nicht verändert werden darf [^1]. Solche Änderungen erzeugen eine Inkonsistenz bei der Verwendung von älteren codierten Daten mit der aktuellen Version des Codesystems. Üblicherweise bekommen solche „inkompatiblen“ Versionsstände des Codesystems unterschiedliche Namen/URI und OIDs um sie auseinanderzuhalten (z.B. die jährlichen Versionen des ICD-10). Nicht alle Codesysteme halten sich in der Praxis an diese Vorgabe. Die ELGA GmbH hebt speziell diese Updates eigens hervor, wir bitten sie hierfür die Updatemeldungen im https://confluence.elga.gv.at/display/SCCTERM/ zu beachten. Bei der Übernahme von Aktualisierungen von solchen Codesystemen ist mit Bedacht vorzugehen.

#### Value Set

Wo immer durch z.B. ELGA CDA Implementierungsleitfäden eine Werteauswahl getroffen wird, wird ein passendes Value Set definiert und mit seinem eindeutigen Namen angegeben. ELGA Value Sets beziehen sich mit wenigen Ausnahmen auf eine bestimmte „Version“ eines oder auch mehrerer Codesysteme, was über den eindeutigen Namen/URI des Codesystemes erkenntlich ist. Dadurch werden die Value Sets unabhängig von der Veränderung der Codesysteme. Darüber hinaus können Value Sets eine eigene Reihenfolge und Baumstruktur (Hierarchie) enthalten.

Sämtliche in den Implementierungsleitfäden verwendeten Value Sets werden hier am österreichischen Terminologie-Browser publiziert. Es gilt für alle österreichischen e-Health Terminologien, dass die Value Sets extensional gehalten werden. Das bedeutet, dass die Konzepte im Value Set explizit gelistet sind und nicht dynamisch mit z.B. Filtern über das Codesystem verlinkt werden. Weiters ist die Expansion des ValueSets stehts vorhanden.

Wie häufig Value Sets geändert werden, hängt von der jeweiligen Anwendung ab. Value Sets, die für „strukturelle“ Elemente benötigt werden (z.B. im CDA-Header, XDS-Metadaten) werden sich selten ändern. „Inhaltliche“ Value Sets (z.B. für Arzneimittellisten, Laboranalysen, Diagnosen-Codierungen) werden sich entsprechend häufig ändern müssen. Hier ist mit **jährlichen** bis **wöchentlichen** Änderungen zu rechnen. In Ausnahmen kann bei der Definition eines Value Sets angegeben werden, dass es nicht geändert oder versioniert werden darf (ValueSet.immutable wird auf true gesetzt).

Bei ELGA Value Sets, die einem regulären Wartungs- und Updatezyklus unterliegen, können Erweiterungen und Änderungen nach fachlicher Prüfung durch den zuständigen Inhaltsverwalter durchgeführt werden (z.B. ELGA Laborparameter, ASP-Liste). Bei anderen inhaltlichen Korrekturen von ELGA Value Sets muss gegebenenfalls die fachliche Entscheidung der Arbeitsgruppe [^2] eingeholt werden, die den entsprechenden Leitfaden entwickelt hat, in dessen Rahmen das Value Set definiert wurde.

Inhalte von Value Sets können sich ändern, der Name und die OID eines Value Sets bleiben aber gleich. Bei neuen Versionen werden Versionsnummer mit Veröffentlichungs-Datum (in ValueSet.version mit z.B.: 2.3.1+20220618) und Änderungsdatum (ValueSet.date) angegeben. Damit kann die Gültigkeit zu einer bestimmten Zeit rekonstruiert werden.

Value Sets sind so lange gültig, bis das Datum einer neueren Version dieses Value Sets erreicht wird – dann gilt die neuere Version. Solange keine neuere Version vorhanden ist, bleibt ein Value Set gültig (für Außnahme "static" siehe auch Kapitel [Value Set Binding](#value-set-binding)). Wenn Codes nicht mehr verwendet werden dürfen, wird eine neue Version des Value Sets erzeugt, in dem die nicht mehr zu verwendenden Codes auf inactive=true gesetzt werden. Diese Codes werden im ValueSet nur aus historischen Gründen behalten. Die neue Version ist ab dem Hochladen gültig, außer der Status des Value Sets wurde auf draft gesetzt und das Datum befindet sich in der Zukunft.

##### Value Set Binding

Für ELGA und den österreichischen eHealth-Systemen gilt grundsätzlich eine DYNAMISCHE Bindung an Value Sets. Das bedeutet, dass immer die aktuell am Terminologieserver publizierte Version eines Value Sets anzuwenden ist. (Das explizite Setzen des entsprechenden Schlüsselworts `DYNAMIC` ist daher in den Leitfäden nicht erforderlich).

Value Sets können auch STATISCH an ein Code-Element gebunden werden. Dies wird durch die Angabe des Value Sets mit Name/URI, OID, Version und Datum (ValueSet.date) sowie dem Schlüsselwort `STATIC` gekennzeichnet.

#### Versionierung

Folgende Versionierung wird erst nach Beendigung des Parallelbetriebs umgesetzt. Solange der alte Terminologieserver gewartet wird, muss sichergestellt werden, dass die Versionierung am alten und neuen Terminologieserver übereinstimmen.

Für die Versionierung von Terminologien wie Codesysteme oder Value Sets gilt folgendes Versionierungsschema:

    MAJOR.MINOR.PATCH+YYYYMMDD

Für einzelne Terminologien wie CodeSysteme oder ValueSets gilt:

* `MAJOR` wird erhöht, wenn z.B.
   * die Intension bzw. Definition der vollständigen Terminologie sich ändert;
* `MINOR` wird erhöht, wenn z.B.
	* ein Konzept hinzugefügt wird;
	* ein Konzept deprecated/retired gesetzt wird;
	* der DisplayName eines Konzepts geändert wird;
   * die Metadaten eines Konzepts sich ändern und damit der Sinn des Konzepts erweitert/geschmälert wird;
   * die Struktur/Gruppierung (z.B. beim ValueSet) sich ändert;
* `PATCH` wird erhöht, wenn z.B.
    * Rechtschreibfehler oder Tippfehler in den Metadaten (nicht DisplayName oder Code) eines vorhandenen Konzepts korrigiert werden.
* `YYYYMMDD` entspricht dem Datum, ab dem die Terminologie gilt.

##### Statusübergangsdiagramm für Konzepte

Folgendens Statusübergangsdiagramm gilt für alle Konzepte in Codesystemen oder Value Sets:

[![status_life_cycle_for_concepts](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/status_life_cycle_for_concepts.png){: style="width: 100%"}](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/status_life_cycle_for_concepts.png)

Dabei ist das Mapping zwischen LOINC® und FHIR® R4 wie folgt:

LOINC↓  FHIR Codesystem →

|  | **Active**&ensp;  | **Deprecated**&ensp; | **Retired**&ensp; | **Experimental**&ensp; |
|---|---|---|---|---|
| **Active** | X |  |  |  |
| **Discouraged** |  | X |  |  |
| **Deprecated** |  |  | X |  |
| **Trial** |  |  |  | X |

Dabei ist das Mapping zwischen SNOMED CT® und FHIR® R4 wie folgt:

SNOMED CT↓  FHIR Codesystem →

|  | **Active**&ensp; | **Deprecated**&ensp; | **Retired**&ensp; | **Experimental**&ensp; |
|---|---|---|---|---|
| **Active** | X |  |  |  |
| **Inactive** |  | X |  |  |


### GitLab-Projektübersicht

Der Inhalt des [österreichischen e-Health Terminologie-Browsers](https://termgit.elga.gv.at/) basiert auf den folgenden zwei GitLab-Projekten:

| Projektname | Beschreibung | Repository-URL | GitLab-Projekt-ID | GitLab-Pages-URL |
| --- | --- | --- | --- | --- |
| TerminoloGit | [https://gitlab.com/elga-gmbh/termgit](https://gitlab.com/elga-gmbh/termgit) | Repository für publizierte, aktuelle Terminologien (Downloadformate).| 33179072 | [https://elga-gmbh.gitlab.io/termgit](https://elga-gmbh.gitlab.io/termgit) <br/><br/>*Hinweis:* Unter dem angegebenen GitLab-Pages-URL werden die Inhalte der letzten erfolgreichen Pipeline eines beliebigen Git-Branches dieses Repositories dargestellt. |
| TerminoloGit HTML | [https://gitlab.com/elga-gmbh/termgit-html](https://gitlab.com/elga-gmbh/termgit-html) | Repository für die statischen HTML-Seiten, die vom HL7® FHIR® IG Publisher auf Basis des `main`-Branches von [https://gitlab.com/elga-gmbh/termgit](https://gitlab.com/elga-gmbh/termgit) erstellt wurden. | 33179017 | **[https://termgit.elga.gv.at](https://termgit.elga.gv.at)** |

### Rollen

Der Terminologieserver ist primär ein System zur Bereitstellung von Codelisten und Value Sets, es ist grundsätzlich kein Echtzeit-Zugriff bei der Verarbeitung durch Informationssysteme vorgesehen. Der Terminologieserver dient derzeit nicht als Online-Ressource (für die Prüfung einzelner Werte), sondern als Quelle für neue Terminologien, die lokal abgespeichert werden sollen.
Der Terminologieserver wird von folgenden Benutzergruppen verwendet:

| Benutzergruppe | Aufgabe | GitLab.com-Rolle | Beschreibung |
| --- | --- | --- | ---|
| Terminologie-Consumer | lesender Zugriff | keine, nicht erforderlich | Als Terminologie-Consumer ist für die Anzeige und den Export von Terminologien bzw. das Überprüfen auf neue Versionen keine Selbstregistrierung notwendig. |
| Terminologie-Verantwortlicher | Terminologie-Wartung | Developer | Die Anlage oder Aktualisierung von Terminologien wird vom Terminologie-Verantwortlichen durchgeführt. Es ist nicht möglich jeder Terminologie einen verantwortlichen Benutzer zuzuordnen. |
| Terminologie-Administrator | Freigabe und Publikation | Maintainer | Bevor Terminologien öffentlich abrufbar werden, erfolgt eine Freigabe durch einen Terminologie-Administrator. |

### Publikationsprozess für Terminologien externer Herausgeber

Für die Publikation von Terminologien, die von ELGA-externen Terminologie-Verantwortlichen für den österreichischen e-Health Terminologieserver erstellt wurden, ist folgender Prozess definiert.

#### Voraussetzungen

- Basiskenntnisse von Git bzw. GitLab werden als bekannt vorausgesetzt.
- Die gewünschte Terminologie unterliegt keinen externen Lizenzbestimmungen und besitzt bereits eine eigene OID. Falls noch keine OID für die Terminologie vorliegt, kann diese über die [OID Plattform](https://www.gesundheit.gv.at/OID_Frontend/application.htm?section=5) beantragt werden.
- Der folgend Erklärte Freigabeprozess und die Vorgehensweise sind bekannt.

#### Freigabeprozess

1. Status "Entwurf" (draft): Nur bestimmte Benutzer dürfen Terminologien anlegen, ändern bzw. importieren. Jede Terminologie hat dafür einen Terminologie-Verantwortlichen. Terminologie-Administratoren können alle Terminologien verändern und technisch freigeben. Alle neu angelegten oder neu importierten Terminologien bzw. Terminologie-Versionen tragen den Status Entwurf/draft und sind nur in einem eigenen Git-Branch sichtbar.
2. Status "zur Freigabe" (draft mit merge request): Der Terminologie-Verantwortliche gibt die Terminologie-Version inhaltlich frei, die Terminologie nimmt dadurch diesen neuen Status an (weiterhin nur in einem eigenen Git-Branch sichtbar, der nun einen Merge-Request gestellt hat).
3. Status "freigegeben" (active): Die erstellten bzw. geänderten Terminologien sind nach einer Freigabe durch einen Terminologie-Administrator auch für Terminologie-Consumer verfügbar (sind in den master/main Git-Branch verschoben worden).
4. Status "ungültig" (retired): Diese Terminologien dürfen nicht (mehr) verwendet werden. Dies kann zwei Auslöser haben:
   1. Der erstellte Entwurf wurde vom Terminologie-Administrator abgelehnt.
   2. Der zugeordnete Terminologie-Verantwortliche oder ein Terminologie-Administrator zieht die Version zurück und setzt sie manuell auf ungültig.

[![Freigabeprozess](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/Freigabeprozess.png "Freigabeprozess"){: style="width: 100%"}](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/Freigabeprozess.png)

#### Vorgehensweise

1. Kontaktaufnahme mit der ELGA GmbH über die E-Mail Adresse [cda@elga.gv.at](mailto:cda@elga.gv.at) mit **[ausgefülltem Antragsformular](files/Applicationform_external_terminology_developer_de.pdf)**:
   1. Name der Terminologie
   2. OID der Terminologie
   3. Codesystem/Value Set
      1. Falls Value Set: Bekanntgabe des/der dazu gehörigen Codesystems/Codesysteme
   4. Beschreibung zur Terminologie (DE und EN)
   5. Verantwortliche Person und Organisation für die Terminologie
      1. Name (Organisation)
      2. E-Mail Adresse (Organisation)
      3. Name (verantwortliche Person)
      4. E-Mail Adresse (verantwortliche Person)
   6. GitLab.com-User, die die Terminologie in das GitLab-Projekt [TerminoloGit](https://gitlab.com/elga-gmbh/termgit) einbringen soll. Die Bekanntgabe mehrerer GitLab.com-User ist möglich.
2. Das ausgefüllte Formular wird von ELGA GmbH technisch und rechtlich geprüft.
3. Nach erfolgreicher Prüfung erhalten die vom Antragsteller genannten GitLab-User "Developer"-Rechte im GitLab-Projekt [TerminoloGit](https://gitlab.com/elga-gmbh/termgit). Damit kann der User einen eigenen Branch erstellen, darf aber ohne Freigabe durch einen User mit "Maintainer"-Rechten nicht in den Default Branch des Projekts mergen.
4. Für das initiale Erstellen der Importdatei werden **Importvorlagen** für **[Codesystem](files/CodeSystem-cs-import-template.1.propcsv.xlsx)** bzw. **[Value Set](files/ValueSet-vs-import-template.1.propcsv.xlsx)** in Form von CSV-Dateien zur Verfügung gestellt. Die benötigten Attribute sind im Abschnitt [Proprietäres CSV](file_formats_de.html#proprietäres-csv-propcsv---csv-und-xlsx) beschrieben.
   1. Das Hochladen in das GitLab-Projekt kann über verschiedenen Wege durchgeführt werden (z.B. GitLab WebIDE oder Software wie z.B. Sourcetree). Für Fragen und Unterstützung kann sich der externe Terminologie-Verantwortliche an das TerminoloGit-Team wenden ([cda@elga.gv.at](mailto:cda@elga.gv.at)).
   2. Pro Branch sollten thematisch zusammenhängende Terminologien bearbeitet werden, damit die Übersicht gewahrt werden kann.
   3. Die Commits müssen der Git-Governance entsprechen: [https://cbea.ms/git-commit/](https://cbea.ms/git-commit/)
   4. Terminologien von externen Terminologie-Verantwortlichen werden unter einer eigenen Kategorie benannt nach dem Organisationsnamen gesammelt.
5. Nach Fertigstellung der Terminologie wird ein Merge Request erstellt, damit der Branch in den Default Branch überführt werden kann.
   1. Der technische Review wird von der ELGA GmbH durchgeführt.
   2. Wenn die technischen Voraussetzungen erfüllt sind, wird der Branch in den Default Branch überführt.
6. Nachdem erfolgreichen Durchlauf der Pipelines wird kontrolliert, ob die gewünschten Terminologien korrekt und vollständig publiziert wurden.
7. Abschließend wird der Terminologie-Verantwortliche über die Publikation informiert und ein Update von der [Changeliste des Semantic Competance Centers](https://confluence.elga.gv.at/display/SCCTERM/Terminologien+-+Changelist+2022) wird veröffentlicht.

### Referenzen

[^1]:Concept Permanence, beschrieben in „Cimino’s Desiderata“ (Desiderata for Controlled Medical Vocabularies in the TwentyFirst Century; 1998; [http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3415631/](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3415631/))
[^2]:  Ein „CDA Beirat“, der Entscheidungen in Umlaufverfahren (qui tacet consentit) trifft. Die getroffenen Entscheidungen können per Mailverteiler publik gemacht werden.

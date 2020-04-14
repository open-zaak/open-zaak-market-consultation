# Onze voorstellen en vragen

| <a href="README.md">Home</a> | <a href="introduction-nl.md">Inleiding</a> | Onze voorstellen en vragen | <a href="how-to-respond-nl.md">Reageren op de marktconsultatie</a> |
| -------- | -------- | -------- | -------- |

Deze pagina bevat drie onderdelen.

1. Een visie voor een open source community - een conceptvisie voor hoe de OpenZaak community eruit zou kunnen zien.
2. Behoeften van gemeenten - een indicatief overzicht van ondersteuningsvormen die gemeenten nodig hebben van leveranciers.
3. Vragen marktconsultatie - een overzicht van onze open vragen aan marktpartijen.

## Visie voor een open source community

Wij geloven dat OpenZaak succesvol is als gemeenten en marktpartijen samen werken aan een gemeenschappelijk doel: een open en samenwerkende community die kan schalen.

Voor gemeenten is het belangrijk om een groot en divers leveranciersnetwerk te hebben, die elke gemeente kan ondersteunen met hun specifieke behoeften (inclusief ondersteuning voor ontwikkeling, hosting en implementatie). Dit zal ook bijdragen aan het verminderen van de risico's van gemeenten bij de implementatie van de OpenZaak codebase.

Voor leveranciers is het belangrijk om het aantal deelnemende gemeenten te laten groeien (de markt voor hun diensten te vergroten) en effectief samen te werken met andere leveranciers (het aanvullen van vaardigheden en het verbeteren van de betrouwbaarheid van de implementatie van de OpenZaak codebase).

Zonder alle antwoorden in detail te kennen, omvat onze visie voor de community:

* samenwerken aan één leverancier-neutrale codebase en shared branchingmodel, waarbij uiteenlopende forks worden vermeden
* collaborative governance, inclusief rond gedeelde roadmaps (feature en technical) en open issue tracker
* een gedeeld inzicht in hoe bugfixes en -ondersteuning kunnen worden aangepakt, met name in situaties van operationele downtime of beveiligingsrisico's
* een inclusieve community (inclusief open communicatiekanalen, codebase marketingmateriaal en codes of conduct) die nieuwe marktpartijen en nieuwe deelnemende gemeenten verwelkomt
* leveranciers in staat stellen om effectieve leden en ambassadeurs van de community te worden

## Behoeften van gemeenten

OpenZaak bestaat uit een set componenten die door gemeenten op diverse wijze gebruikt zullen worden. Dit betekent dat de gemeenschap moet worden ingericht om verschillende soorten leveranciers in staat te stellen verschillende soorten gemeenten te ondersteunen.

De onderstaande lijsten beschrijven eerst de behoeften die alle gemeenten zullen hebben, en vervolgens drie 'soorten' gemeenten en hun bijbehorende behoeften ten opzichte van de community en marktondersteuning.

### Behoeften die alle gemeenten hebben

* Er moeten koppelingen zijn met externe databases/sets (i.e. basisgegevens)
* Er is de behoefte om de eigendom over data te behouden, en continue toegang tot die data te hebben
* Er is eenvoudige dataportabiliteit nodig (bijvoorbeeld voor wettelijk vereiste archivering)
* Er zijn leveranciers nodig die bijdragen aan de main repository van OpenZaak (inclusief [EUPL-licentie](https://github.com/open-zaak/open-zaak/blob/master/LICENSE.md))
* Er is de behoefte om in lijn te blijven met de [VNG-standaarden](https://www.vngrealisatie.nl/producten/api-standaarden-zaakgericht-werken)
* Er is de behoefte om de feature roadmap te beïnvloeden
* Er is behoefte dat leveranciers OpenZaak opnemen in al hun zaak systemen en andere zaak-gerichte producten en aanbiedingen

### Behoefte aan ‘Full service' pakket

Sommige gemeenten hebben behoefte aan een full service pakket. Dit omvat hosting, implementatie, onderhoud en ontwikkeling, door een of meerdere leveranciers. Daarnaast wordt OpenZaak geïntegreerd met bestaande producten van bestaande leveranciers, bijvoorbeeld de zaaksystemen die ze gebruiken.

Zij hebben leveranciers nodig die het volgende aanbieden:

* hosting support
* implementation support
* maintenance support
* new feature en bug fix support
* integration support
* helpdesk, configuration support, vragen en training
* bug fixes en hot fixes

### Behoefte aan 'Backend as a service'

Sommige gemeenten hebben een 'Backend as a service' nodig. Ze zijn in staat om andere applicaties, die afhankelijk zijn van OpenZaak, op hun eigen servers (of in de cloud) te draaien, maar willen dat leveranciers OpenZaak voor hen hosten, uitvoeren en onderhouden.

Zij hebben leveranciers nodig die het volgende aanbieden:

* een integratie partner
* duidelijke continuous integration/continuous development
* een sandbox environment
* bug fixes en hot fixes
* helpdesk, configuration support, en treining

### Behoefte aan In-house implementatie

Sommige gemeenten zullen OpenZaak met uitsluitend eigen middelen willen implementeren. Zij zullen hun werk moeten coördineren met andere gemeenten en leveranciers.

Zij moeten in de community samenwerken aan:

* duidelijke development/contribution guidelines
* samenwerken met marktpartijen en andere gemeente omtrent een product en technical roadmap en backlogs
* een manier om bug fixes te coordineren met marktpartijen en andere gemeente

## Vragen marktconsultatie

Deze sectie bevat een lijst met open vragen. Elk deel bevat onze huidige veronderstellingen en een reeks open vragen die we willen bespreken met de leveranciersgemeenschap.

Let op: vragen zijn indicatief, we horen graag uw mening over elk van de punten in deze bijlage.

### 1. Single shared codebase

#### Veronderstellingen

We willen een open community op schaal faciliteren, inclusief samenwerking op een vendor- neutrale codebase en shared branching model, waarbij uiteenlopende forks worden vermeden. Dit willen we opnemen in de contracten die gemeenten hebben met leveranciers, bijvoorbeeld door het benoemen van afspraken over branches en een nadruk op continuous integration.

#### Vragen

1. Hoe zou u dit principe willen opnemen in contracten die gemeenten met u afsluiten?
2. Hoe stelt u voor om 'soft forks' up-to-date te houden van elkaar? Moet er een centrale repository zijn die als master kan worden beschouwd?
3. Welke uitdagingen zijn er voor u om in zo'n multi-branch omgeving te werken? Hoe kunnen deze uitdagingen worden beperkt om de bedrijfsrisico's voor u te verminderen?
4. Heeft u ooit eerder op deze manier gewerkt?
5. Is de [huidige architectuur en make-up van de codebase](https://github.com/open-zaak/open-zaak) bevorderlijk voor multi-vendor samenwerking en modulaire implementatie van componenten?

### 2. Shared codebase governance

#### Veronderstellingen

Onze visie is om samenwerking mogelijk te maken tussen meerdere gemeenten en leveranciers, die samen aan de codebase werken. Hiervoor is een gedeeld bestuur nodig voor de codebase. Dit kan onder meer het volgende behelzen: a) een open en gedeelde issue en bug tracker, b) een open en gedeelde feature roadmap, en c) een open en gedeelde technical roadmap. Dit omvat ook engineering en contributing guidelines, evenals open communicatiekanalen.

Deze marktconsultatie omvat een [ontwerpvoorstel van een governancestructuur](governance.md) voor open discussie.

#### Vragen

1. Hoe vindt u dat governance moet worden georganiseerd binnen de community?
2. Wat zijn de uitdagingen die u voorziet bij het onderhouden van open backlogs bij uw klanten?
3. Wie moet verantwoordelijk zijn voor het bijwerken van de shared roadmap? U, de gemeenten, of een gedeelde verantwoordelijkheid?
4. Hoe wilt u de gedeelde feature en technical roadmap kunnen beïnvloeden?
5. Hoe wilt u dat de community omgaat met het ontwikkelen, eens worden en onderhouden van gedeelde engineering en contributing guidelines?
6. Welke risico’s ziet u in het werken in zo'n omgeving?

### 3. Bugs en bug fixes

#### Veronderstellingen

Er zal een centrale, openbare en geprioriteerde issue tracker zijn voor features en bugs. Veel van deze problemen kunnen kleine hoeveelheden werk (minder dan 80 uur) omvatten. Daarnaast zullen veel gemeenten issues en bugs hebben die verband houden met hun lokale implementatie en context.

#### Vragen

1. Moet het werken op zowel lokale implementaties en de centrale repository worden opgenomen in de zelfde of aparte contracten?
2. Hoe wilt u dat de contracten zo gestructureerd zijn dat u kunt werken aan lokale implementaties en branches en ook kunt bijdragen aan de centrale repository?
3. Hoe moeten bugfixes in de hele community worden geïmplementeerd? Kunnen leveranciers hotfixes van andere leveranciers overnemen voordat deze zijn samengevoegd in de centrale repository? Of moeten leveranciers pas wijzigingen doorvoeren nadat ze zijn samengevoegd in de centrale repository?
4. Wat voor soort aansprakelijkheidsvraagstukken zouden er kunnen zijn indien ‘hot fixing’ onverwachte schade of verdere problemen oplevert? Levert dit een probleem op voor uw contractuele verplichtingen aan uw klant?

### 4. Helpdesk en support

#### Veronderstellingen

Veel gemeenten zullen de voorkeur geven aan één enkele leverancier die ze kunnen bellen voor al hun behoeften. Dit varieert van vragen, bugs, ideeën voor doorontwikkeling, technische integratie, training, configuratie van machtigingen / autorisatie, meldingen, enzovoort. Onze veronderstelling is dat in veel gevallen, geen enkele leverancier al deze diensten kan of wil leveren.

#### Vragen

1. Is het mogelijk om één helpdesk op te zetten voor alles wat te maken heeft met het gebruik van OpenZaak door een gemeente? Of zijn er voordelen voor verschillende leveranciers die verschillende helpdesks onderhouden voor verschillende soorten vragen (bijvoorbeeld om hen in staat te stellen hun serviceaanbod te differentiëren?)
2. Kunnen meerdere marktpartijen zich verenigen om hun aanbod te combineren?
3. Kunnen gespecialiseerde 'helpdeskaanbieders' werk uitbesteden aan andere aanbieders?

### 5. Standards compliance

#### Veronderstellingen

De OpenZaak API's zijn gebaseerd op een VNG standaard, de [API's voor zaakgericht werken](https://www.vngrealisatie.nl/producten/api-standaarden-zaakgericht-werken). De standaard wordt continu onderhouden en verbeterd en OpenZaak moet daaraan blijven voldoen. Deze updates moeten worden gepropageerd over de centrale repository-branche, evenals repositories die marktpartijen gebruiken om hun diensten te leveren (zoals backend-as-a-service).

#### Vragen

1. Hoe zorgen we ervoor dat updates van de VNG-standaard op de juiste manier worden doorgevoerd in lopende OpenZaak-implementaties? Moeten deze vereisten worden opgenomen in contracten met marktpartijen?
2. Wat vindt u van versiebeheer van OpenZaak ten opzichte van andere toepassingen? Hoeveel backwards-compatible versies moeten worden ondersteund?
3. Moeten leveranciers in het kader van hun contracten worden gevraagd om wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak te laten bijdragen aan de VNG-standaard?

### 6. Codebase marketing

#### Veronderstellingen

Om de community effectief te laten schalen, gaan we ervan uit dat er een set neutraal marketingmateriaal moet zijn, waaronder logo, website, productdocumentatie, casestudies, business case materiaal, enzovoort. Wij zijn van mening dat dit leveranciers- en gemeente- neutraal moet zijn om een gedeelde set storytelling resources mogelijk te maken.

#### Vragen

1. Op welke wijze zou u willen dat dit marketingmateriaal wordt gemaakt?
2. Wat voor invloed wilt u hebben op dit materiaal en de website?
3. Moeten leveranciers contractueel worden gevraagd om, wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak, toe te voegen aan het OpenZaak marketingmateriaal (inclusief bijvoorbeeld user testimonials, business cases, etc)?

| <a href="README.md">Home</a> | <a href="introduction-nl.md">Inleiding</a> | Onze voorstellen en vragen | <a href="how-to-respond-nl.md">Reageren op de marktconsultatie</a> |
| -------- | -------- | -------- | -------- |

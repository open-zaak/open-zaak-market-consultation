# Introductie

Geachte heer Lindeboom, beste Niels,

Maykin Media is opgericht in 2008 en wij zijn specialisten op het gebied van de ontwikkeling en beheer van webapplicaties, koppelvlakken en websites met behulp van open source software, met maatwerk als kracht en Agile/Scrum als methode.

Met een team van ontwikkelaars hebben wij met veel plezier gewerkt aan OpenZaak en vinden het prachtig om te zien hoe een open source project op deze manier professioneel ondersteund gaat worden om zo alle gemeenten van dienst te kunnen zijn, en de Common Ground transitie in de praktijk te brengen.

Wij zijn voornemens om OpenZaak aan te bieden als dienst op ons cloud platform, maar ook te ondersteunen middels consultancy en installaties op locatie. Dit kan voor zowel gemeentes als andere leveranciers die OpenZaak gebruiken in hun eigen oplossingen.

In de afgelopen 12 jaar hebben wij veel succesvolle projecten gedaan voor partijen zoals de Belastingdienst, het Ministerie van Financiën, Logius, Vereniging Nederlandse Gemeenten (VNG) en diverse gemeenten maar ook voor Artis, IKEA, de Anne Frank Stichting en Booking.com. Van de meeste projecten doen wij tevens tot op heden het beheer, onderhoud en doorontwikkeling. OpenZaak past hier prima bij en delen van OpenZaak komen juist voort uit door ons ontwikkelde open source componenten uit eerdere projecten.

Bijgevoegd vindt u onze antwoorden op de vragen uit de marktconsultatie. Wij zijn altijd bereid onze antwoorden toe te lichten.


# Algemeen

De insteek van een open marktconsultatie via Github en de type vragen zijn vooruitstrevend en passend bij een open source product en het toekomstbeeld van Common Ground. Mooi om te zien!

We zien het voorgestelde model als iets om naar toe te groeien en in potentie generiek toepasbaar op allerlei producten. De producten in een gegevenslandschap zijn geen grote suites meer. De vraag of de opzet daardoor niet iets te groot wordt neergezet komt daarom wel bij ons boven drijven maar wordt in de vragen verder toegelicht.

Verder ontbreekt het commerciële belang van de huidige stakeholders. Waarom doet Dimpact dit, waarom doen de gemeenten dit? En hoe vind financiering van OpenZaak uberhaupt plaats en hoe schaalt dat als meer gebruikers komen? Hoe kunnen gebruikers van OpenZaak er op vertrouwen dat er budget blijft om door te ontwikkelen?

Dit soort vragen rondom de visie van Dimpact op OpenZaak en het borgen dat OpenZaak een blijvend succes wordt zijn zaken die bij ons als leverancier leven, en waar we graag (naast jullie eigen vragen) met jullie van gedachten over wisselen.

 
# Single shared codebase

## Veronderstellingen

*We willen een open community op schaal faciliteren, inclusief samenwerking op een vendor- neutrale codebase en shared branching model, waarbij uiteenlopende forks worden vermeden. Dit willen we opnemen in de contracten die gemeenten hebben met leveranciers, bijvoorbeeld door het benoemen van afspraken over branches en een nadruk op continuous integration.*

## Vragen

1. **Hoe zou u dit principe willen opnemen in contracten die gemeenten met u afsluiten?**

Het gaat een beetje in tegen het community idee maar volgens ons moeten hier harde afspraken over worden vastgelegd in contracten. Deze afspraken zouden eventueel als artikel/contract template kunnen worden aangeboden vanuit OpenZaak.

Het basis idee moet zijn dat alle aanpassingen/wijzigingen/features die buiten de master repository plaatsvinden worden aangeboden aan de master repository. Het is dan aan OpenZaak (wie en wat dat dan ook precies is, komt later) om deze aanbieding (pull request) te reviewen en op te nemen, af te wijzen, of aanpassingen te vragen.

OpenZaak stelt vervolgens de review richtlijnen op die, los van verdere afspraken/contracten, altijd kunnen worden gewijzigd (versoepeld/strenger).

2. **Hoe stelt u voor om 'soft forks' up-to-date te houden van elkaar? Moet er een centrale repository zijn die als master kan worden beschouwd?**

De open-zaak/open-zaak repository is in onze ogen de master repository en daarmee de centrale plek van de codebase. Het voordeel voor gemeentes is dat er 1 centrale plek is waar alle features en bugfixes uiteindelijk samenkomen. Het voordeel voor leveranciers is dat ze altijd naar 1 plek kunnen kijken voor updates, roadmap, versies e.d. Het landschap wordt erg ingewikkeld en onoverzichtelijk als er meerdere "master repositories" zijn.

Soft-forks zijn waarschijnlijk onoverkomelijk. Immers, een leverancier wil een bepaalde feature er soms snel in hebben en niet wachten op een nieuwe release van OpenZaak. Als deze feature uiteindelijk in OpenZaak wordt opgenomen is de soft-fork niet meer nodig.

Er ontstaat wel een probleem als deze feature bijvoorbeeld afgewezen wordt door OpenZaak. Er is nu een versie met deze feature en zonder deze feature. Het is nu de verantwoordelijkheid van de maker van de soft-fork om deze up-to-date te houden met de features/fixes in de master repository. 

Een concrete afspraak kan bijvoorbeeld zijn dat als de master-repository een nieuwe versie released, dat elke leverancier binnen 1 kwartaal deze ook moet aanbieden. Dat geldt dan ook voor diegenen die een soft-fork aanbieden.

Het mag ook niet zo zijn dat een leverancier een soft-fork versie aanbied EN een master versie, en alleen klanten met de master versie voorziet van de laatste updates. Updates op de master branch moeten beschikbaar worden voor alle klanten onafhankelijk van de fork anders krijg je gemeenten die noodgedwongen achter blijven op nieuwe versies van de ZGW APIs.

3. **Welke uitdagingen zijn er voor u om in zo'n multi-branch omgeving te werken? Hoe kunnen deze uitdagingen worden beperkt om de bedrijfsrisico's voor u te verminderen?**

Onze gedachte is om altijd de master (laatste officiële versie) aan te bieden. 

Afwijken is technisch niet handig en economisch onvoordelig. Als de gemeente die de afwijkende versie persé wil hebben zal die ook voor alle kosten opdraaien. Wij zouden dit dus afraden en vanwege de eenvoud alle gemeenten mee laten groeien in de verdere ontwikkeling van OpenZaak.

4. **Heeft u ooit eerder op deze manier gewerkt?**

Als deze vraag betrekking heeft op vraag 3 dan is het antwoord nee. Idealiter dient altijd voorkomen te worden dat er veel afwijkende producten leven iets wat naar onze mening voor OpenZaak zeker niet nodig is maar meer van toepassing zal zijn op applicaties in de bovenste Common Ground laag.

Mocht deze vraag betrekking hebben op de veronderstellingen, dan is het antwoord ja. We maken gebruik van vele open source pakketten die we gebruiken waarbij forks mogelijk zijn (en soms ook tijdelijk doen) maar we vooral op de hoofd branch zitten. Continuous integration en het werken met branches, versies, e.d. van onze eigen software is onderdeel van onze standaard werkwijze.

Het hebben van een uitgebreide testsuite met CI maakt het up-to-date blijven en het onderhouden van soft-forks relatief gezien eenvoudig.

5. **Is de huidige architectuur en make-up van de codebase bevorderlijk voor multi-vendor samenwerking en modulaire implementatie van componenten?**

Ja, want:

   1. Geschreven in een van de populairste programmeertalen ([bron](https://www.tiobe.com/tiobe-index/)).
   2. Een testsuite die 96% van de code doorloopt ([bron](https://codecov.io/gh/open-zaak/open-zaak) en [bron](https://travis-ci.org/github/open-zaak/open-zaak)).
   3. Ontwikkelaar, systeembeheerder en functionele documentatie beschikbaar ([bron](https://open-zaak.readthedocs.io/en/latest/)).
   4. Geteste REST API’s volgens de API standaarden van VNG ([bron](https://api-test.nl/server/1/224fd5be-bc64-4d55-a190-454bee3cc8e3/14bc91f7-7d8b-4bba-a020-a6c316655e65/latest/)).
   5. Code wordt automatisch gecontroleerd op leesbaarheid en codestijl ([bron](https://travis-ci.org/github/open-zaak/open-zaak)).

OpenZaak is een set API’s die als microservice kan worden gebruikt in een landschap dat bestaat uit bronnen ontsloten door API’s en applicaties die deze API’s gebruiken.

Ten slotte wordt het geheel aangeboden als Docker containers waarmee heel veel zaken worden weg geabstraheerd zodat beheer, leveren een aanbieden van OpenZaak relatief eenvoudig is en enkel kennis vereist van OpenZaak zelf en Docker.

Het werken met testsuites, reviews, code quality, Docker containers, Kubernetes en open source software, sluit wel heel nauw aan bij hoe wij werken. We zijn daarom benieuwd naar hoe andere leveranciers hier tegen aankijken.

# Shared codebase governance

## Veronderstellingen

*Onze visie is om samenwerking mogelijk te maken tussen meerdere gemeenten en leveranciers, die samen aan de codebase werken. Hiervoor is een gedeeld bestuur nodig voor de codebase. Dit kan onder meer het volgende behelzen: a) een open en gedeelde issue en bug tracker, b) een open en gedeelde feature roadmap, en c) een open en gedeelde technical roadmap. Dit omvat ook engineering en contributing guidelines, evenals open communicatiekanalen.*

*Deze marktconsultatie omvat een ontwerpvoorstel van een governancestructuur voor open discussie.*

## Vragen

1. **Hoe vindt u dat governance moet worden georganiseerd binnen de community?**

In essentie is het ontwerpvoorstel prima maar hier moet in onze ogen naar toe gegroeid worden indien nodig. Wellicht kan er kleiner begonnen worden e.e.a. afhankelijk van bijvoorbeeld een eerste aanzet tot een roadmap door de gemeenten.

Grotere uitbreidingen/features zullen wellicht in een eigen/ander product worden vormgegeven.

Het is verder onduidelijk wie/welke organisaties er in het product steering team zitten. In onze ogen zouden dit de organisaties moeten zijn die OpenZaak gebruiken en dat deze, door voldoende capaciteit beschikbaar te maken, de teams van OpenZaak in stand houden. Er ontstaat een soort vereniging rondom OpenZaak en/of breder.

In dit stadium is het naar onze mening beter om met een "huispartij" te werken die de richting bepaalt op basis van het product steering team en dit elke zoveel tijd te evalueren, om te komen tot een technical steering team. Als er afgestemd moet worden tussen verschillende leveranciers ontstaat een soort werkgroep als vanouds wat de voortgang kan frustreren. 

2. **Wat zijn de uitdagingen die u voorziet bij het onderhouden van open backlogs bij uw klanten?**

Issues die worden ingeschoten bij ons door een klant, kunnen een verwijzing krijgen naar een issue bij OpenZaak. De enige uitdaging is dat wij als leverancier niet volledig "in control" zijn over de afhandeling van dit issue. Bewustzijn en expectation management bij klanten is hiervoor essentieel.

3. **Wie moet verantwoordelijk zijn voor het bijwerken van de shared roadmap? U, de gemeenten, of een gedeelde verantwoordelijkheid?**

Gedeelde verantwoordelijkheid maar het Product Steering team zal de eindverantwoordelijke zijn.

4. **Hoe wilt u de gedeelde feature en technical roadmap kunnen beïnvloeden?**

Dit moet volgens ons 1 roadmap worden. Techniek staat in dienst van de functionaliteit.
Invloed uitoefenen middels stem uitbrengen en onderwerpen kunnen aandragen (als issue? waar dan op gestemd kan worden).

5. **Hoe wilt u dat de community omgaat met het ontwikkelen, eens worden over en onderhouden van gedeelde engineering en contributing guidelines?**

Voor de korte termijn lijkt het ons handig om 1 partij aan te wijzen die de doorontwikkeling verzorgt en beslissingen neemt totdat de community groter is. Dit zou bijvoorbeeld halfjaarlijks geëvalueerd worden om naar het gewenste model te groeien.

6. **Welke risico’s ziet u in het werken in zo'n omgeving?**

De risico’s zijn beperkt maar onenigheid over beslissingen kan leiden tot onrust en publieke schade. Uiteindelijk kunnen hard-forks ontstaan of kan een leverancier "aan de haal gaan" met de code en zo de governance omzeilen. Er komt dan defacto een nieuwe master en dat schept weer verwarring. Voldoende budget, snelle reacties en inspelen op de vraag zijn essentieel om de leiderschap en het vertrouwen in OpenZaak te behouden.

# Bugs en bug fixes

## Veronderstellingen

*Er zal een centrale, openbare en geprioriteerde issue tracker zijn voor features en bugs. Veel van deze problemen kunnen kleine hoeveelheden werk (minder dan 80 uur) omvatten. Daarnaast zullen veel gemeenten issues en bugs hebben die verband houden met hun lokale implementatie en context.*

## Vragen

1. **Moet het werken op zowel lokale implementaties en de centrale repository worden opgenomen in de zelfde of aparte contracten?**

Wellicht is het handig om het wel in hetzelfde contract op te nemen middels een bijlage. Zo’n bijlage kan OpenZaak beschikbaar stellen en stelt de basis regels op over het omgaan met issues die betrekking hebben op OpenZaak. Dit maakt het voor gemeenten en leveranciers duidelijk dat er gewerkt wordt met een afhankelijkheid/component dat elders betrokken wordt.

2. **Hoe wilt u dat de contracten zo gestructureerd zijn dat u kunt werken aan lokale implementaties en branches en ook kunt bijdragen aan de centrale repository?**

Eigen branches (van soft-forks) worden idealiter altijd aangeboden aan de master repository zodat het OpenZaak team kan beslissen of dit wenselijk is voor alle gemeenten. Dit hoeft niet direct maar hier kan een termijn voor worden opgenomen en alleen als het een branch/soft-fork betreft die ook echt bij de klant draait. Test branches e.d. hoeven niet te worden ingediend uiteraard.

3. **Hoe moeten bugfixes in de hele community worden geïmplementeerd? Kunnen leveranciers hotfixes van andere leveranciers overnemen voordat deze zijn samengevoegd in de centrale repository? Of moeten leveranciers pas wijzigingen doorvoeren nadat ze zijn samengevoegd in de centrale repository?**

Leveranciers moeten uitgaan van de centrale repository. Dat sluit niet uit dat leveranciers bug fixes of features die nog niet in de master branch zitten, niet kunnen gebruiken. We zouden hiervoor geen restricties opnemen.

4. **Wat voor soort aansprakelijkheidsvraagstukken zouden er kunnen zijn indien ‘hot fixing’ onverwachte schade of verdere problemen oplevert? Levert dit een probleem op voor uw contractuele verplichtingen aan uw klant?**

Als wij de laatste master repository versie van OpenZaak als dienst of als component aanbieden van onze oplossing en er gaan bijvoorbeeld gegevens verloren, dan zal de gemeente ons mogelijk aansprakelijk stellen voor schade en zullen wij kosten moeten maken om e.e.a. te repareren.

Er zijn 2 scenario’s:

   1. Een leverancier biedt OpenZaak aan als "los" component.
   2. Een leverancier biedt een product aan dat gebruik maakt van Open Zaak als onderdeel van haar product.

In scenario 1: Een leverancier biedt OpenZaak als dienst aan en neemt daarmee verantwoording over de dienst die zij aanbiedt. Deze leverancier zal zelf verantwoordelijk zijn een hotfix eerst goed te testen en/of minimaal backups gereed hebben van voor de hotfix.

In scenario 2: Dit is vergelijkbaar met het gebruik gebruik van software bibliotheken bij open source of niet open-source producten. De aanbieder/beheerder van het product is verantwoordelijk en niet de maker van de software bibliotheek.

Eventuele risico’s kunnen verwerkt worden in de service kosten. Een goede acceptatie procedure, keten-testsuite en backups (ofwel de kwaliteit en omvang van de service) zijn daarnaast essentieel om problemen te voorkomen.

# Helpdesk en support

## Veronderstellingen

*Veel gemeenten zullen de voorkeur geven aan één enkele leverancier die ze kunnen bellen voor al hun behoeften. Dit varieert van vragen, bugs, ideeën voor doorontwikkeling, technische integratie, training, configuratie van machtigingen / autorisatie, meldingen, enzovoort. Onze veronderstelling is dat in veel gevallen, geen enkele leverancier al deze diensten kan of wil leveren.*

## Vragen

1. **Is het mogelijk om één helpdesk op te zetten voor alles wat te maken heeft met het gebruik van OpenZaak door een gemeente? Of zijn er voordelen voor verschillende leveranciers die verschillende helpdesks onderhouden voor verschillende soorten vragen (bijvoorbeeld om hen in staat te stellen hun serviceaanbod te differentiëren?)**

Wij zien voor ons een 1e lijn helpdesk bij de gemeente zelf, 2e lijn bij de aanbieder van OpenZaak, 3e lijn bij het OpenZaak team. Dit is een soort trechter van vragen maar ook in grootte. Per gemeente, per leverancier en ten slotte 1 helpdesk van OpenZaak zelf.

Elke gemeente heeft zijn eigen mensen die kunnen helpen. Elke leverancier kent zijn eigen pakket (evt. in combinatie met OpenZaak) het beste. Als de leverancier er niet uit komt kan die de vraag inschieten bij OpenZaak.

2. **Kunnen meerdere marktpartijen zich verenigen om hun aanbod te combineren?**

Het mooie van Common Ground is juist dat aanbod niet door marktpartijen hoeft te worden gecombineerd (met speciale koppelingen e.d.) maar dat gemeenten dit kunnen doen omdat componenten uitwisselbaar zijn. Uiteraard kan dit wel met ondersteuning van weer een derde partij die faciliteerd bij integraties.

Er zullen partnerships ontstaan, zoals dat ook nu al het geval is, van partijen met elk hun specialisme. Dit uit zich dan in oplossingen die producten van verschillende leveranciers combineren.

Er is 1 belangrijk verschil met deze partnerships in het geval van open source en dat is dat er geen licentiekosten mee gemoeid zijn. Een leverancier A die nu product X van leverancier B aanbiedt, betaalt licentiekosten waarmee leverancier B geld ontvang voor doorontwikkeling van product X. In het geval van open source kan leverancier A het product zelfstandig, en zonder kosten, gaan aanbieden. Hierdoor is een partnership met een partij die gespecialiseerd is in product X minder noodzakelijk.

3. **Kunnen gespecialiseerde 'helpdeskaanbieders' werk uitbesteden aan andere aanbieders?**

Lijkt ons van wel maar we hebben hier geen directe ervaring mee.

# Standards compliance

## Veronderstellingen

*De OpenZaak API's zijn gebaseerd op een VNG standaard, de API's voor zaakgericht werken. De standaard wordt continu onderhouden en verbeterd en OpenZaak moet daaraan blijven voldoen. Deze updates moeten worden gepropageerd naar de centrale repository-branche, evenals repositories die marktpartijen gebruiken om hun diensten te leveren (zoals backend-as-a-service).*

## Vragen

1. **Hoe zorgen we ervoor dat updates van de VNG-standaard op de juiste manier worden doorgevoerd in lopende OpenZaak-implementaties? Moeten deze vereisten worden opgenomen in contracten met marktpartijen?**

Het past niet goed bij open source maar ervaring leert helaas dat dit niet zomaar gaat gebeuren, dus ja, eisen in contracten.

2. **Wat vindt u van versiebeheer van OpenZaak ten opzichte van andere toepassingen? Hoeveel backwards-compatible versies moeten worden ondersteund?**

Het is ons onduidelijk of API-versies of OpenZaak versies worden bedoeld.

Voor OpenZaak raden wij een eenvoudig versiemodel aan: De laatste versie heeft de meeste features en bugfixes. Er worden geen versies parallel onderhouden: Als OpenZaak 1.0 en 2.0 bestaat zal niet bij een 2.0.1 versie ook een 1.0.1 versie nog worden gereleased.

Wat betreft versies raden wij aan het VNG model aan te houden, dat is "vrijwel" onderdeel van de standaard. Minimaal de laatste en voorlaatste major versies blijven beschikbaar en maximaal 1 major versie update per jaar. Een voorbeeld:

In OpenZaak 1.2 zit nu Zaken API 1.0. Als Zaken API 2.0 wordt gereleased wordt in OpenZaak 1.3 zowel Zaken API 1.0 als 2.0 beschikbaar. Als later Zaken API 3.0 uitkomt, dan zal in OpenZaak 1.4 alleen Zaken API 2.0 en 3.0 beschikbaar zijn. Aangenomen dat er verder geen versie updates zijn geweest in OpenZaak.

Dit betekent wel dat als je als gemeente persé Zaken API 1.0 wil hebben, dat je vast zit aan OpenZaak met de maximale versie 1.3. Op deze versie worden dan ook geen bugfixes meer gedaan, want die zitten in 1.4.x. In het uiterste geval kan deze leverancier wel zelf bugfixes in 1.4.x backporten naar 1.3.x (die dan weer open source beschikbaar komt).

3. **Moeten leveranciers in het kader van hun contracten worden gevraagd om wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak te laten bijdragen aan de VNG-standaard?**

Ja, maar vrijwillig en VNG moet hier een toegankelijk proces voor hebben. Het gebeurt nu helaas te weinig dat informatie wordt uitgewisseld. De Github van VNG en OpenZaak laten al zien dat er wel feedback komt op beslissingen maar een extra incentive zou goed zijn, zoals bij VNG de API-labs deden.

# Codebase marketing

## Veronderstellingen

*Om de community effectief te laten schalen, gaan we ervan uit dat er een set neutraal marketingmateriaal moet zijn, waaronder logo, website, productdocumentatie, casestudies, business case materiaal, enzovoort. Wij zijn van mening dat dit leveranciers- en gemeente- neutraal moet zijn om een gedeelde set storytelling resources mogelijk te maken.*

## Vragen

1. **Op welke wijze zou u willen dat dit marketingmateriaal wordt gemaakt?**

Volledig aan gemeenten/Dimpact die het weer in samenspraak met de technische steering team kan afstemmen. Een goede technische context is bij marketing essentieel om geen verkeerde dingen te communiceren, maar het moet geen technisch verhaal worden.

Wij zien hier ook een rol voor het OpenZaak team, als voorloper in de Common Ground transitie, om het gebruik van verschillende componenten van verschillende leveranciers te promoten. Dit zorgt voor een gezonde markt, voordeligere prijzen voor gemeenten, en betere werking tussen componenten van verschillende leveranciers.

2. **Wat voor invloed wilt u hebben op dit materiaal en de website?**

Middels issues verzoek kunnen indienen op Github zou prima werken maar niet alles hoeft langs alle leveranciers of teamleden te gaan.

Het is wellicht buiten scope maar een overzicht van aanbieders zou gemeenten helpen om een keuze te maken. Grotere leveranciers zullen snellers suites aanbieden waar OpenZaak een onderdeel van is. Dit is vaak wel de makkelijkere keus voor gemeenten maar bevordert niet de component gedachte van Common Ground.

3. **Moeten leveranciers contractueel worden gevraagd om, wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak, toe te voegen aan het OpenZaak marketingmateriaal (inclusief bijvoorbeeld user testimonials, business cases, etc)?**

Op basis van producten en casestudies zou het heel mooi zijn als leveranciers materiaal 'neutraal' beschikbaar zouden willen stellen. Omgekeerd moet het marketing materiaal van OpenZaak ook door leveranciers gebruikt kunnen worden voor marketing doeleinden. OpenZaak kan dit stimuleren door vragen/templates beschikbaar stellen om dit uit te vragen/in te dienen.

Wel moet opgepast worden, dat als testimonials worden opgenomen, er niet een soort impliciete review site ontstaat van leveranciers. Dat lijkt ons buiten scope en zet nieuwe partijen vrij snel buiten spel wat de markt ontoegankelijk maakt.

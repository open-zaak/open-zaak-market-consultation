Beste initiatiefnemers van OpenZaak,

Hartelijk dank voor de uitnodiging aan ons om mee te doen met de marktconsultatie OpenZaak. Onderstaand treft u onze visie en beeld op de ontwikkelingen waarover we graag verder met u in gesprek gaan.

In 2017 heeft de VNG de ambitie neergelegd om meer grip te krijgen op het gemeentelijke ICT-landschap en de daarbij behorende applicaties. Dit initiatief, Common Ground, heeft als doel de gemeentelijke informatiehuishouding op orde brengen en daarmee de dienstverlening naar een hoger niveau te tillen. Dit wil men bereiken door niet langer (verschillende versies van dezelfde) informatie op verschillende plekken te hebben staan. Het kopiëren en synchroniseren van informatie tussen verschillende applicaties moet stoppen. Opslag vindt plaatst bij de bron, waar elke applicatie telkens zijn informatie ophaalt. Een andere reden die vaak aangehaald wordt is dat men niet langer afhankelijk wil zijn van (‘grote’) leveranciers of applicaties in gebruik wil hebben waar men ‘niet vanaf kan’. Hiervoor is het nodig dat data en de applicatie van elkaar gescheiden worden. Data mag niet langer in de ‘leveranciers silo’ zitten. Het moet mogelijk zijn om op elk moment de ene applicatie te vervangen voor de andere applicatie (met min of meer dezelfde functionaliteit, maar bijvoorbeeld totaal andere gebruikersinterface). Dit kun je natuurlijk alleen bereiken als je een bepaalde mate van standaardisatie doorvoert in de markt.

Uiteraard is het werken met standaarden voor gegevensuitwisseling niet nieuw in de gemeentelijke markt. Zo kennen wij StUF, ofwel het Standaard Uitwisseling Format. In 2006 werden de leden van de VNG geïnformeerd over het nastreven van het gebruik van StUF-XML voor de gegevensuitwisseling en het realiseren van koppelingen op basis van StUF-XML. Het doel: betere dienstverlening aan burgers en bedrijven. In 2013 kwam daar een vastgestelde Zaak- en Documentservices versie 1.0 bij. Deze ZaakDMS-standaard ondersteunt het zaakgericht werken en de noodzaak om zaaksystemen en documentmanagementsystemen goed op elkaar aan te laten sluiten. Uiteraard is óók zaakgericht werken een middel om te komen tot betere dienstverlening door resultaatgerichte processen te gebruiken.

Kijkend naar het huidige gemeentelijke ICT-landschap en het initiatief uit 2017 om de Common Ground te starten, laat zien dat het gemeentelijk ICT-landschap zich nog niet optimaal heeft gevormd. Standaarden blijken toch geen standaarden als elke leveranciers het anders interpreteert. Het huidige landschap wordt gekend door kopiëren en synchroniseren van gemeentes, waarbij niet altijd elke applicatie tijdig op de hoogte is van de meest actuele informatie. Dit zorgt soms voor vervelende situaties in dienstverlening aan burgers en bedrijven. En deze manier van koppelen en synchroniseren maakt het onnodig duur (informatie herhaaldelijk opslaan vraagt nu eenmaal meer geheugencapaciteit) en complex (welke koppelingen zijn waar gelegd, wanneer wordt alles bijgewerkt?).

Om te komen tot een gemeentelijke informatievoorziening die bijdraagt aan de dienstverlening, en gemeentes meer flexibiliteit en grip en geeft op hun gegevenslandschap heeft de Common Ground een aantal uitgangspunten. Allereerst, de leveranciers silo’s verdwijnen, en data wordt van de applicatie gescheiden en éénmalig opgeslagen voor meervoudig gebruik.

Het enkelvoudig gebruik van informatie uit de bron, de landelijke registraties, zorgt ervoor dat elke medewerker, met elke applicatie altijd de actuele informatie beschikt. Deze data wordt ontsloten via application programming interfaces (kortweg API’s genoemd), kleine stukjes software die specifiek bedoelt zijn om gegevens te ontsluiten. De integratielaag (NLX) zorgt ervoor dat applicaties, zoals het zaaksysteem en andere gemeentelijke backoffice applicaties, op een veilige en vertrouwde manier gebruik kunnen maken van deze gegevens. Het betreft hier niet alleen gegevens van de organisatie zelf, de integratielaag zorgt er tevens voor dat gegevens van andere organisaties ontsloten kunnen worden.

Om de werking van de Zaakgericht Werken (ZGW) API’s aan te tonen is er meer nodig dan alleen een ‘technische’ application programming interface. Er moet ook daadwerkelijk een interface komen, die een eindgebruiker, bijvoorbeeld iemand vanuit vergunningverlening, kan gebruiken. Er zijn in de fieldlabs die de Common Ground ontwikkelingen hebben gefaciliteerd verschillende werkgroepen geweest die deelproducten hebben opgeleverd. Zo is het framework waarop de ‘Common Ground’ draait ontwikkelt (de NLX, Haven), maar ook ‘eindgebruiker’ applicaties die de ZGW API’s implementeren. OpenZaak is één van deze resultaten. Het doel van OpenZaak is een productiewaardige implementatie van de ZGW API’s. Oftewel een software component, met interface, die in de basis gebruikt kan worden voor zaakbehandeling. OpenZaak is een open source codebase gebouwd in opdracht van een coalitie van meer dan 45 gemeenten waaronder Dimpact.

Het andere uitgangspunt van OpenZaak, maar ook van Common Ground, en inmiddels onderschreven door staatssecretaris Binnenlandse Zaken, is vrijgeven van broncode van overheidssoftware.

Inmiddels lijkt OpenZaak-community op zoek te zijn naar leveranciers met kennis en capaciteit om de ontwikkelde software door te ontwikkelen, hosten, onderhouden en implementeren. Dit zijn bij voorkeur meerdere leveranciers die de open source gedachte, community ontwikkeling en het EUPL(model) ondersteunen. Daarnaast moet er rekening gehouden worden dat OpenZaak is ontwikkelt met Python. Leveranciers die geen ervaring hebben met deze programmeertaal moeten hier rekening mee houden en de extra kosten die dit met zich mee brengt. Daarnaast is het ingewikkeld om een leveranciers community te vormen rondom al ontwikkelde code. Hoewel niet onmogelijk, hebben we in de praktijk gezien dat het lang kan duren (bijv. Eclips). En daarnaast zien we vooral Open Source modellen voor Operating systems of middleware componenten en generieke frameworks.

Maar eerst moet duidelijk worden hoe deze community vormgegeven kan worden. De marktconsultatie OpenZaak vraagt input op diverse aspecten die van belang zijn bij het werken volgens open source modellen. Zoals vormgeving van contracten met gemeentes, governance structuren vaststellen van functionele en technische roadmaps, het omgaan met wijzigingen in standaarden en oplossen van bugs. Vragen én antwoorden die meerdere leveranciers van proprietary software hebben ingevuld vanuit hun huidige ‘closed source’ business modellen. En die volgens de open source, community, filosofie ingevuld moet worden door de Stichting achter OpenZaak.

Zaaksysteemleveranciers en andere leveranciers van gemeentelijke oplossingen onderschrijven het belang van nieuwe standaarden die niet multi-interpretabel zijn. Daarnaast zien we de ontwikkeling en behoefte om deze oplossingen open source aan te bieden. Maar dit reist wel de vraag hoe je het onderhoudt en de borging van dit stuk open source software gaat organiseren. Vaak zie je een stichting die borgt dat de open source software onderhouden wordt. Deze stichting huurt ontwikkelaars, of bedrijven, in om dit onderhoud voor hun uit te voeren. Hierbij rijst de vraag hoe de stichting wordt voorzien van de middelen om dit te financieren.

Voor partijen die deze rol willen vervullen is het belangrijk dat zij een business case zien in het onderhouden en doorontwikkelen van een productiewaardige referentie implementatie van de ZGW API’s (OpenZaak). Hoe organiseer je als stichting voor deze partij een gegarandeerde inkomstenstroom?

Belangrijk is daarbij te benoemen dat OpenZaak ontwikkelt is onder de EUPL, European Union Public License. Dit EUPL is een ‘copyleft’ licentiemodel wat betekent de broncode, origineel, aangepast of verbeterd ten alle tijden weer openbaar gemaakt moet worden. De vraag is dan ook tot hoe ver deze EUPL reikt. Heeft dit tevens impact op leveranciers die met hun interfaces aansluiten op OpenZaak, en deze applicaties bij voorkeur als proprietary aanbieden. Is dit mogelijk binnen de filosofie en het licentiemodel van OpenZaak? En kunnen de partijen die verantwoordelijk worden voor het onderhoud van de OpenZaak software zich ook gaan richten op het ontwikkelen van applicatie interfaces waarmee zij zich onderscheiden, en kan dit dan propretairy aangeboden worden? Of krijgen we daarmee een belangenconflict wanneer zij ervoor kunnen kiezen om dat stuk onderhoud of doorontwikkeling te doen op het stuk Open Source software, waarbij die partij gebaad is? Of moeten de partijen die OpenZaak onderhouden op zoek naar andere manieren om hun inkomsten aan te vullen?

Het lijkt erop dat binnen het EUPL model weinig tot geen ruimte is voor het creëren van additionele functionaliteit vanuit een eigen inzicht en, daarmee ook risicovol, dit onder closed source licentie weg te zetten, omdat de OpenZaak community verwacht dat de doorontwikkeling eigendom wordt van de community, d.w.z. open source beschikbaar wordt. Simpelweg omdat deze additionele functionaliteiten gebruik maken van en voortbouwen op bestaande broncode die volgens de EUPL dan weer openbaar moet zijn. Het is dan ook de vraag of dit niet innovatie in de weg staat.

Dan is er nog de mogelijkheid van het leveren van aanvullende diensten, denk daarbij aan implementatie van de software of ondersteuning bij het gebruik van software en/of de hosting van de software. Dit zou een mogelijkheid kunnen zijn voor de partijen die het onderhoud op zich nemen om extra inkomsten te genereren. In dat geval zal een gemeente die gebruik maakt van de OpenZaak software één van de leveranciers contracteren die hen zal ondersteunen bij de bovengenoemde aspecten. Alleen wat weerhoudt adviesbureaus, ZZP’ers en andere marktpartijen zich ervan om zonder deel uit te maken van de community zich ook op te werpen als implementatiepartner van OpenZaak software? Mogelijk kunnen zij dit zelf goedkoper aanbieden omdat zij de ontwikkel- en onderhoudskosten van OpenZaak niet voor hun rekening nemen (ze zijn geen lid van de community of ‘slapend’ lid) dan de partijen die én ontwikkelen én onderhouden en deze investering middels hun diensten terug moeten verdienen. Daarnaast is het maar de vraag of de ondersteuning bij implementatie nodig is, of dat een (groot) deel van de gemeentes voldoende kennis en kunde in huis heeft om OpenZaak zelf van GitHub te halen en dit zelf te installeren. Het is immers vrij te downloaden, en neemt zelfs de noodzaak weg voor gemeentes om te betalen voor software dat hun zaakgericht werken ondersteunt. Dit levert in elk geval geen inkomsten op voor de Stichting om het onderhoud te kunnen bekostigen. Wel is de vraag of je dan naar een licentiemodel/contract wil toegaan waarbij gemeentes voor het melden van bugs of ontvangen van support een bedrag afdragen aan de stichting. Zoals bijvoorbeeld Alfresco toepast.

Daarnaast zijn de initiatiefnemers op zoek naar een ‘gezonde leveranciers community’, waarin leveranciers de mogelijkheid krijgen om de markt voor OpenZaak te laten groeien, en waarin inkoop wordt vereenvoudigd en gestandaardiseerd. Volgens ons houdt dit ook in dat er een diverse pool aan leveranciers participeert in deze community. Daarbij is de vraag hoe je deze leveranciers gemotiveerd krijgt én houdt om te participeren. Zolang deze leveranciers private bedrijven zijn, zullen ze naast een technologisch en impact motief ook geleid worden met een (gedeeltelijk) commercieel motief. Een privaat bedrijf, is op basis van een gezonde business case intrinsiek te motiveren om open source software te ontwikkelen (en te onderhouden!). Er zullen voldoende inkomsten tegenover moeten staan. En zelfs als de gemeentes die gebruik maken van OpenZaak een substantiële financiële bijdragen leveren aan de Stichting achter OpenZaak, en dit gedistribueerd wordt onder de deelnemers, is er een risico of dit voldoende inkomsten genereerd om dit onderhoud te financieren. Zeker wanneer men “gemeente de kans biedt om in eigen tempo en op eigen voorwaarde de overstap te maken”. En het dus nog maar de vraag is wie, wanneer gebruik gaat maken van OpenZaak. Het is niet zeker dat de 45 participerende gemeentes in het OpenZaak project uiteindelijk ook daadwerkelijk afnemer worden van OpenZaak.

Eigenlijk zou de community vergroot moeten worden en er een wereldwijde community gecreëerd moeten worden met CASE management als Nederlands export product. Dit vergroot de kans dat de stichting voldoende inkomsten kan genereren om het onderhoud te bekostigen. Het verleden met o.a. MMBase leert dat een puur Nederlands open source initiatief door de schaal lastig vorm te geven is. Daarnaast zien we op Europees niveau meerdere soort gelijken initiatieven ontstaan. Zo is in Vlaanderen het uitgangspunt voor overheidssoftware ook open source. Maar zij vragen partijen via aan aanbesteding componenten te ontwikkelen die daarna open source worden vrijgegeven. Het onderhoud en stukje doorontwikkeling wordt nog een aantal jaren bij de ontwikkelde partij gelegd waar zij ook voor betaald worden. Dit levert echter nog wel de vraag in hoe een divers landschap aan leveranciers hierin voort kan bestaan. Of moeten zij ook op zoek naar andere markten waarin zij meer waarden kunnen creëren middels andere verdienmodellen? Het is daarom ook interessant om na te gaan welke Europese of wereldwijde initiatieven er al zijn rondom case management waarbij kan worden aangesloten. Of op zoek te gaan hoe de community buiten de overheidsmarkt uitgebreid kan worden.

In onze optiek zou OpenZaak zich moeten concentreren tot het niveau van een interface met functionaliteit onder water. Op de interface met de gebruiker kunnen leveranciers zich onderscheiden, en waar je in de markt ook de concurrentie op wil zien. Het gebruiksgemak en de gebruikersinterface en investeringen in business rules en gebruikersfunctionaliteit.

Het is daarbij dus vooral interessant om met de community de API’s te ontwikkelen. Zo zorg je samen voor standaarden in gegevensuitwisseling en interoperabiliteit. De verwachting is echter dat bij de gemeentes de vraag blijft bestaan naar extra informatie en gegevens die nog niet ondersteund worden door de ontwikkelde open source API’s. Het kan dus dat een leverancier gevraagd wordt deze API te ontwikkelen, of een leverancier ziet zelf een latente behoefte en ontwikkelt op eigen initiatief deze API. Hoe dan ook, de vraag is hoe deze innovatieve doorontwikkeling gefinancierd wordt. In het eerste geval zouden de ontwikkeluren voor het ontwikkelen van de API betaald kunnen worden door de vragende gemeente(s), en daarna, deels in lijn met de beleidsbrief van staatssecretaris Knops, als open source beschikbaar worden gesteld (alleen de API, niet de implementatie in de applicatie die deze API gebruikt).

Echter, de vraag is wat je doet met de API’s en applicatie die is ontwikkelt naar aanleiding van de latente behoefte die de leverancier zag. De leverancier heeft in dit geval een risico genomen en wordt daarmee al dan niet beloond door afname. Licentiemodellen onder proprietary software hebben hierin de voorkeur om dit risico te financieren. En open source beschikbaar stellen, ook van de API, nadat er één gemeentelijke afnemer is van het product verlaagd de stimulans om vernieuwend bezig te zijn. Dit betekent dat de innovatie binnen de gemeentelijke markt vraaggestuurd blijft. Op zich niet erg, maar zal vaak niet leiden tot echte vernieuwing, omdat het vaak gaat om verbeteringen van wat we al doen en kennen (incrementele innovatie) en niet zoveel radicaal of disruptief. Het zou zo moeten zijn, voor een optimaal functionerend ecosysteem, dat van zzp’er tot groter softwarehuis zou moeten kunnen en willen investeren voor eigen risico. Software investering met een voldoende interessant terugverdienmodel dat in relatie staat tot het genomen risico.

Erg benieuwd zijn wij naar de mogelijke aanbesteding die wordt genoemd. Is het correct dat de stichting achter OpenZaak op zoek is naar partijen die het onderhoud op zich willen nemen? Want, wanneer het uitgangspunt is Open Source development middels een community, hoe past hier dan een aanbesteding bij, waarin vaak een exclusief recht wordt gegeven aan de aanbestedende partij? Wie is de opdrachtgever? Om welk recht gaat dit dan, wie zijn de klanten en wat willen ze precies bereiken? Is dit puur en alleen een partij die de implementatie doet van OpenZaak? Of gaat dit ook om doorontwikkeling van OpenZaak? En kun je dat wel aanbesteden als het juist vanuit de community en Open Source ontwikkelt moet worden of wordt de wetgeving hierop worden aangepast dat aanbesteding eenvoudiger kan?

**Onze conclusie:**<br>
Wellicht dat een licentiemodel, en focus op het community based ontwikkelen van de API’s, én niet de implementaties hiervan, de markt brengt waar het wil zijn. Daarnaast is het de verwachting dat het nodig is de scope van OpenZaak als open source case management oplossing te vergroten om zo een voldoende grote potentiele afzetmarkt te genereren, waarmee ook voldoende inkomsten naar de stichting kunnen gaan waaruit het onderhoud bekostigd kan worden. Belangrijk uitgangspunt blijft uiteraard gegevens ophalen bij de bron, ontsloten via standaarden. Verschillende applicaties ontwikkeld door diverse leveranciers. De gemeente kiest die applicaties waar het niet meer vanaf wil (maar wel kan) en daarmee haar dienstverlening naar een hoger niveau tilt.

**OpenZaak en Exxellence**<br>
Wij staan positief tegenover het aansluiten op de OpenZaak API’s en hebben hier ook in samenwerking met gemeente Utrecht een implementatie met onze Exxellence Suite op gerealiseerd. Wij zijn onze Exxellence Suite aan het decomponentiseren zodat we zowel ons eigen Zakenmagazijn alsmede OpenZaak kunnen ondersteunen.

Daarnaast zetten wij deze gedachte verder door, door het ontwikkelen van een nieuw taakspecifiek platform (www.ellensoftware.nl). Hiermee geven wij invulling aan de behoefte voor kleine functionele applicaties. En wij doen op dit moment ervaring op met Amazon Webservices. De interactie met OpenZaak API’s en onze ontwikkelingen willen wij graag verder onderzoeken. Hierbij is het wel belangrijk om precies duidelijk te hebben wat de impact van de EUPL is.

Om tot een gedetailleerde invulling en beantwoording te komen van de vragen uit de marktconsultatie, is het nodig om een grondige analyse te doen van de community rondom OpenZaak, de doelstellingen, en de mogelijke financieringsvormen. Ook is het zinvol om diverse verschillende licentiemodellen en toepassingen bij andere open source software producten met elkaar te vergelijken en hier lessen uit te trekken.

De gegeven antwoorden geven een richting van onze denkwijze, maar om tot concrete invulling over te gaan is het nodig deze analyse samen verder op te pakken en hier met elkaar over in gesprek te gaan.

Bijgevoegd een verdere beantwoording op de gestelde vragen in de marktconsultatie rondom specifieke onderwerpen.

Bovenstaande zienswijze lichten we graag toe en gaan we graag verder met u over in gesprek in de door u aangekondigde workshops.

Met vriendelijke groet,

Vivette van Cooten<br>
Productmanager

Michel Veenhuis<br>
CEO

**Antwoorden vragen markconsultatie OpenZaak**

**1. Single shared codebase**

**Veronderstellingen**<br>
We willen een open community op schaal faciliteren, inclusief samenwerking op een vendor- neutrale codebase en shared branching model, waarbij uiteenlopende forks worden vermeden. Dit willen we opnemen in de contracten die gemeenten hebben met leveranciers, bijvoorbeeld door het benoemen van afspraken over branches en een nadruk op continuous integration.

**Vragen**

1. Hoe zou u dit principe willen opnemen in contracten die gemeenten met u afsluiten?<br>
*Dit zou georganiseerd kunnen worden door een OpenZaak community voorwaarden document op te stellen waarnaar verwezen kan worden en waarmee opdrachtgever en opdrachtnemer dienen in te stemmen. Dit in lijn met zoals het met de GIBIT ook gebeurd is. Echter is het wel de vraag of je contracten kunt afsluiten als software open source is, en dus vrij te downloaden.*

2. Hoe stelt u voor om 'soft forks' up-to-date te houden van elkaar? Moet er een centrale repository zijn die als master kan worden beschouwd?<br>
*Er is een centrale master benodigd waarop een transparant proces voor contributie wordt geborgd volgens binnen de community geldende guidelines. Met daarin ook duidelijke eindverantwoordelijke die bepaald of de pull requests voldoen.*

3. Welke uitdagingen zijn er voor u om in zo'n multi-branch omgeving te werken? Hoe kunnen deze uitdagingen worden beperkt om de bedrijfsrisico's voor u te verminderen?<br>
*De uitdaging kan zitten in het niet tijdig en eenduidig op de centrale branch doorgevoerde wijzigingen die benodigd zijn voor ontwikkelen die er een afhankelijkheid mee hebben. Er is een eigenaar van de code, maintainer, nodig die strak te regie houdt op de multi-branches. Daarnaast is het de verantwoordelijkheid van de contributors dat men het tijd commit en de hoofdbrache in de gaten houdt.*

4. Heeft u ooit eerder op deze manier gewerkt?<br>
*Exxellence en haar voorloper Emaxx hebben zelf in de begintijd een open source BPEL Engine ontwikkeld. Daarnaast is de MidOffice Suite in de begin tijd gedeeltelijk onder een GPL licentie geleverd en gepubliceerd op ook het OSOSS platform van de Nederlands overheid. Ook maakt Exxellence veelvuldig gebruik van open source middleware componenten. Exxellence heeft met gemeenten rondom (open) standaarden mee geholpen de Zaak-DMS standaard te initiëren en te ontwikkelen.*

5. Is de huidige architectuur en make-up van de codebase bevorderlijk voor multi-vendor samenwerking en modulaire implementatie van componenten?<br>
*Dit is lastig te overzien op dit moment met de ervaring die we nu hebben met deze code. We denken dat we dit met een aantal concullega bedrijven zouden moeten testen in de praktijk om ervaring op te doen.*

**2. Shared codebase governance**

**Veronderstellingen**<br>
Onze visie is om samenwerking mogelijk te maken tussen meerdere gemeenten en leveranciers, die samen aan de codebase werken. Hiervoor is een gedeeld bestuur nodig voor de codebase. Dit kan onder meer het volgende behelzen: a) een open en gedeelde issue en bug tracker, b) een open en gedeelde feature roadmap, en c) een open en gedeelde technical roadmap. Dit omvat ook engineering en contributing guidelines, evenals open communicatiekanalen.
Deze marktconsultatie omvat een ontwerpvoorstel van een governancestructuur voor open discussie.

**Vragen**

1. Hoe vindt u dat governance moet worden georganiseerd binnen de community?<br>
*Er moet voldoende samenhang alsmede autonomie bij de verschillende gemeenten en leveranciers blijven. De richtlijnen voor de community moeten helder en transparant met de community worden vormgegeven. Een externe audit partij zou hierop onafhankelijk toezicht kunnen houden. Extra aandacht vragen we voor hoe om gegaan moet worden met overheidsstandaarden en compliancy als de DigiD audit, NEN 2082, webrichtlijnen. Hoe borg je dat open source software hier aan voldoet, en wat betekent dit voor implementaties die klanten zelf doen? Het governance model van Apache kan inzicht geven.*

2. Wat zijn de uitdagingen die u voorziet bij het onderhouden van open backlogs bij uw klanten?<br>
*Op dit moment werken we reeds met open backlogs reeds met onze opdrachtgevers. De uitdaging zit op dat gemeenten verschillende onderdelen willen realiseren waar minder samenhang in is. Het gezamenlijk prioriteren van dezelfde ontwikkelingen blijkt lastig te zijn. Als de community groot genoeg wordt aan zowel gemeente als leverancier (gemeente en software partijen) zijde wordt dit probleem mogelijk minder. Wel is belangrijk helder te hebben wie verantwoordelijk is voor het maken van de keuzes en uiteindelijke prioritering. Dit kan bij de Stichting liggen, eventueel uitbesteed aan een derde partij. Goed moet worden nagedacht of dit dezelfde partij kan zijn die het onderhoud doet. En of deze partij wel of geen aanvullende software producten kan leveren op basis van OpenZaak. Mogelijk geeft dit een belangenconflict, of worden keuzes en prioriteit uiteindelijk bepaald door de agenda van het bedrijf dat óók inkomsten genereerd door het leveren van extra producten. Ook hiervoor kan het Apache model extra inzicht bieden.*

3. Wie moet verantwoordelijk zijn voor het bijwerken van de shared roadmap? U, de gemeenten, of een gedeelde verantwoordelijkheid?<br>
*Hier ligt een gedeelde verantwoordelijkheid bij de community. Zie het Apache model voor eventuele inzichten hierop.*

4. Hoe wilt u de gedeelde feature en technical roadmap kunnen beïnvloeden?<br>
*Op de technical roadmap zouden we graag veel invloed willen kunnen uitoefenen. De feature roadmap zou meer vanuit de gemeente kant bepaald kunnen worden.*

5. Hoe wilt u dat de community omgaat met het ontwikkelen, eens worden over en onderhouden van gedeelde engineering en contributing guidelines?<br>
*Dit zou een efficiënt en transparant proces moeten zijn waarbij de goede balans tussen centrale sturing en autonomie bij de verschillende deelnemers ontstaat. Het Apache model kan hiervoor interessante elementen bevatten.*

6. Welke risico’s ziet u in het werken in zo'n omgeving?<br>
*Hoe houdt je een community werkbaar zonder teveel overhead en overlegstructuur is een aandachtspunt. Verder zal bij teveel consensus mogelijk middelmaat ontstaan en bij te veel centrale sturing kan het zijn dat partijen (leveranciers en gemeenten) zich er niet meer in herkennen en een eigen stroming en weg inslaan.*

**3. Bugs en bug fixes**

**Veronderstellingen**<br>
Er zal een centrale, openbare en geprioriteerde issue tracker zijn voor features en bugs. Veel van deze problemen kunnen kleine hoeveelheden werk (minder dan 80 uur) omvatten. Daarnaast zullen veel gemeenten issues en bugs hebben die verband houden met hun lokale implementatie en context.

**Vragen**
1. Moet het werken op zowel lokale implementaties en de centrale repository worden opgenomen in de zelfde of aparte contracten?<br>
*Verantwoordelijkheid lokale implementatie ligt bij de gemeente zelf. Dit is geregeld in het open source model. Bugs kunnen ook daar opgelost worden. Dit betekent wel dat deze oplossingen terug geleverd moeten worden aan de community. Echter de acceptatie en implementatie ligt bij de maintainer. Dit brengt wel beduidend risico met zich mee voor de gemeente. Zij kunnen hun eigen weg in slaan om de OpenZaak implementatie passend te maken voor hun omgeving en aansluiting op andere applicaties, maar mogelijk vraagt elke update van OpenZaak opnieuw maatwerk.*

2. Hoe wilt u dat de contracten zo gestructureerd zijn dat u kunt werken aan lokale implementaties en branches en ook kunt bijdragen aan de centrale repository?<br>
*Alles wat je lokaal aanpast en verbetert, lever je terug. Alleen is het geen garantie dat dit onderdeel gaat uitmaken van de mainbranche. Dit kan in de toekomst problemen geven wanneer je naar een hogere versie van de OpenZaak software gaat, en daarbij ‘oude bugs’ in de lokale implementatie opnieuw opgelost moeten worden. Dit moet een bewuste keuze zijn van de gemeente en zij moeten zich dit risico goed realiseren. Ook dit is onderdeel van het open source model.*

3. Hoe moeten bugfixes in de hele community worden geïmplementeerd? Kunnen leveranciers hotfixes van andere leveranciers overnemen voordat deze zijn samengevoegd in de centrale repository? Of moeten leveranciers pas wijzigingen doorvoeren nadat ze zijn samengevoegd in de centrale repository?<br>
*Dit brengt veel risico met zich mee. Je wilt die via gestandaardiseerd release meenemen en hier duidelijk over communiceren. Dit kan uiteindelijk leiden tot maatwerk. De vraag is hoe de community hier mee om wil gaan. Hier zou het Linux model input kunnen leveren.*

4. Wat voor soort aansprakelijkheidsvraagstukken zouden er kunnen zijn indien ‘hot fixing’ onverwachte schade of verdere problemen oplevert? Levert dit een probleem op voor uw contractuele verplichtingen aan uw klant?<br>
*Dit is contractueel af te dichten denken wij en is te ondervangen in werkwijzes rondom releasing. Hotfixing vermijden, goede acceptatie en productie cyclus bij de implementatie partij is van belang. Echter bedenk ook dat de aangesloten applicatie gelijktijdig mee moeten moet. Dit brengt substantiële kosten met zich mee voor de leveranciers van deze applicaties en de gebruikers van deze applicaties. Hoe worden deze kosten gedekt?*

**4. Helpdesk en support**

**Veronderstellingen**<br>
Veel gemeenten zullen de voorkeur geven aan één enkele leverancier die ze kunnen bellen voor al hun behoeften. Dit varieert van vragen, bugs, ideeën voor doorontwikkeling, technische integratie, training, configuratie van machtigingen / autorisatie, meldingen, enzovoort. Onze veronderstelling is dat in veel gevallen, geen enkele leverancier al deze diensten kan of wil leveren.

**Vragen**
1. Is het mogelijk om één helpdesk op te zetten voor alles wat te maken heeft met het gebruik van OpenZaak door een gemeente? Of zijn er voordelen voor verschillende leveranciers die verschillende helpdesks onderhouden voor verschillende soorten vragen (bijvoorbeeld om hen in staat te stellen hun serviceaanbod te differentiëren?)<br>
*Het is mogelijk om een eerstelijns helpdesk centraal in te richten en hier 2e en 3e lijns support van andere leveranciers mee aan te sturen. Ik denk dat we zeker behoefte hebben om te kijken of we ook de totale behoefte af kunnen dichten met de groep softwarebedrijven die we aan het opbouwen zijn. Wij zouden graag een menukaart ontwikkelen waarbij gemeenten kunnen kiezen of en welke diensten ze bij ons af zouden willen nemen.*

2. Kunnen meerdere marktpartijen zich verenigen om hun aanbod te combineren?<br>
*Dat kan zeker en goed gaan werken wanneer de chemie en synergie tussen partijen goed is en de verhoudingen enigszins gelijk. Wel zouden wij graag nog een toelichting op deze vraag en de gedachte hierachter horen, zodat we hier verder over kunnen sparren in bijvoorbeeld een workshop.*

3. Kunnen gespecialiseerde 'helpdeskaanbieders' werk uitbesteden aan andere aanbieders?<br>
*Ook dat is mogelijk en in te richten en centraal aan te sturen. We denken wel dat randvoorwaardelijk is dat de 1e lijns helpdesk dan dusdanig van skills voorzien is dat het goede analyses kan doen ook inhoudelijk en het niet functioneert als alleen maar doorgeefluik.*

**5. Standards compliance**

**Veronderstellingen**<br>
De OpenZaak API's zijn gebaseerd op een VNG standaard, de API's voor zaakgericht werken. De standaard wordt continu onderhouden en verbeterd en OpenZaak moet daaraan blijven voldoen. Deze updates moeten worden gepropageerd naar de centrale repository-branche, evenals repositories die marktpartijen gebruiken om hun diensten te leveren (zoals backend-as-a-service).

**Vragen**

1. Hoe zorgen we ervoor dat updates van de VNG-standaard op de juiste manier worden doorgevoerd in lopende OpenZaak-implementaties? Moeten deze vereisten worden opgenomen in contracten met marktpartijen?<br>
*Dit zou onderdeel kunnen zijn van voorwaarden waaraan partijen zich committeren bij deelname aan de community. Dit geldt dan zowel voor gemeenten als leveranciers. Daarnaast is een certificering wenselijk waarmee gecontroleerd wordt of de implementaties voldoen aan de specificaties.*

2. Wat vindt u van versiebeheer van OpenZaak ten opzichte van andere toepassingen? Hoeveel backwards-compatible versies moeten worden ondersteund?<br>
*In onze optiek zou dit idealiter N-1 moeten zijn. In de praktijk zou bij uitzondering N-2 toegestaan moeten worden. Wel blijft het gelijktijdig updaten van de aangesloten applicaties van groot belang, maar ook een grote uitdaging. Enerzijds lijkt de Common Ground beweging aan te sturen op een nog diverse markt met meer taakapplicaties en meer leveranciers. Daarmee wordt het updaten van aangesloten applicaties een grote operationele en financiële aangelegenheid voor de gemeente. Is men zich hiervan bewust?*

3. Moeten leveranciers in het kader van hun contracten worden gevraagd om wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak te laten bijdragen aan de VNG-standaard?<br>
*Het vrijwillig delen van dit soort ervaringen is zeer nuttig en zou grote toegevoegde waarde kunnen hebben dat dit door VNG meegenomen wordt in het opstellen en doorontwikkelen van de standaarden.*

6. Codebase marketing

**Veronderstellingen**<br>
Om de community effectief te laten schalen, gaan we ervan uit dat er een set neutraal marketingmateriaal moet zijn, waaronder logo, website, productdocumentatie, casestudies, business case materiaal, enzovoort. Wij zijn van mening dat dit leveranciers- en gemeente- neutraal moet zijn om een gedeelde set storytelling resources mogelijk te maken.

**Vragen**

1. Op welke wijze zou u willen dat dit marketingmateriaal wordt gemaakt?<br>
*Het zou mooi zijn als OpenZaak in haar uitingen een neutraal en ingetogen logo en huisstijl aanhoudt. Dit maakt het voor leveranciers mogelijk dit goed in te passen en te hergebruiken in hun uitingen. Daarnaast zouden de leveranciers die actief meedoen een prominente plek moeten krijgen in de uitingen. Met name het mee kunnen gaan met de communicatie kanalen over nieuwe ontwikkelingen zou prettig zijn. Daarnaast een actieve marktplaats en positionering van ontwikkelde add-on modules en applicaties zou een verrijking van de community kunnen zijn. De domeinnaam openzaak.nl zou eigendom moeten zijn van de stichting en niet van een commerciële marktpartij.*

2. Wat voor invloed wilt u hebben op dit materiaal en de website?<br>
*Beperkte invloed. Als leverancier beschikken we over eigen marketing mensen. Met name de vrijheid om in onze eigen marketing ook het OpenZaak initiatief mee te kunnen nemen.*

3. Moeten leveranciers contractueel worden gevraagd om, wat ze hebben geleerd bij het implementeren en ondersteunen van OpenZaak, toe te voegen aan het OpenZaak marketingmateriaal (inclusief bijvoorbeeld user testimonials, business cases, etc)?<br>
*Dit gaan leveranciers uit zich zelf wel doen om zich te profileren. Dit contractueel vastleggen heeft niet per se toegevoegde waarde.*

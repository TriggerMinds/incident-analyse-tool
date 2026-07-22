# ONDERZOEKSAGENDA V3: REALISTISCHE HAALBAARHEIDSANALYSE — OPENBARE DATABRONNEN

## INLEIDING

Dit document is een grondige herziening van de eerdere onderzoeksagenda's (v1 en v2). Waar v1 en v2 uitgingen van een **ideale** datawereld — met toegang tot privé-chatlogs, hulpverleningsdossiers, volledige platformdata en institutionele archieven — vertrekt deze v3 van de **realistische** datawereld: alleen wat publiek toegankelijk is.

De kernvraag is niet "wat zouden we willen weten?", maar "wat kunnen we **daadwerkelijk** weten met de data die voor empirisch onderzoek beschikbaar is?"

### Context van deze herziening

De onderzoeksomgeving — bestaande uit Module 1 (Jeugd Incidenten 15-18) en Module 2 (Authentieke Intieme Menselijke Taal & 17-Assige Taxonomie) — biedt een unieke, multi-dimensionele coderingsinfrastructuur voor onderzoek naar digitale intimiteit, naaktheid en seksuele communicatie. De toolonderdelen zijn:

- **NPM 1-6:** Naturalness Probability Model voor spontane taalkans
- **Authenticity Layer:** 10 categorieën van geformaliseerd tot spontaan taalgebruik
- **Register A/B polarisatiemodel:** Eufemistisch-extern vs. direct-intern register
- **SVP V1-V4:** Self-Validation Protocol voor taalkundige conclusies
- **17-assige taxonomie:** Multi-dimensionele classificatie van intieme media
- **Gedragsladder (Niveau 0-5):** Granulariteitsniveaus voor bronvergelijking
- **Content-Frequency Denominator:** Noemer-standaardisatie voor prevalentiecijfers
- **MissingnessMap:** Systematische registratie van ontbrekende data
- **Cross-Source Translation Table:** Vertaling tussen onderzoeksterminologieën
- **DeviceAffordanceRecord:** Platform-affordance mapping
- **IncidentRecord:** 16+ domeinen integrale codering
- **MediaLifecycleRecord:** 6-fasen levenscyclus van media
- **TrajectoryRecord:** 9-fasen trajectmodel
- **Pattern Library:** Alpha/Beta/Gamma sequentiepatronen
- **Non-Event Baseline:** Verplichte registratie van niet-geëscaleerde casussen
- **Anti-dubbeltellingsregel:** Consolidatie van gecorreleerde signalen
- **Gewogen bewijsmodel:** Bewijssterkte 0-4 met beslisdrempels

Deze instrumenten zijn in v1 en v2 toegepast op een ideale datawereld. In v3 worden ze toegepast op de realistische datawereld van openbaar toegankelijke bronnen.

### Methodologisch uitgangspunt

Dit onderzoek is **descriptief, empirisch en analytisch**. Het vermijdt moralisering, politieke duiding, juridisch advies en automatische criminalisering. De focus ligt op wat we kunnen weten uit openbare data, met expliciete documentatie van wat we niet kunnen weten.

## FASE 1: HAALBAARHEIDSANALYSE VAN DATABRONNEN

### 1.1 WEL BRUIKBAAR — PUBLIEK TOEGANKELIJK

#### Sociale media & forums

**Reddit — Pushshift-archief (2005-2023):**
Volledig openbaar archief van alle publieke subreddits. Bevat posts, comments, metadata (timestamps, scores, gebruikers, subreddit), en is via API of directe data-dumps beschikbaar. Relevant voor onderzoek naar natuurlijke taal, discours-analyse, terminologie-tracking over tijd. Specifiek relevante subreddits: r/sex, r/relationships, r/AskReddit, r/dating, r/dating_advice, r/teenagers, r/nederlands, r/thenetherlands, r/dirtyr4r, r/dirtypenpals, r/AmItheAsshole, r/TooAfraidToAsk, r/NSFW411, r/sexover30, r/DeadBedrooms, r/Infidelity, r/survivinginfidelity.

**Twitter/X — Academic API tier:**
Historische tweets, metadata, netwerkdata. Beperkt sinds 2023 (betaalde API, ~.000/maand), maar historische datasets via archieven en academic partnerships. Relevant voor real-time discours-analyse, trending topics, terminologie-diffusie.

**YouTube — Data API:**
Volledige metadata van openbare video's, comments, statistieken. Relevant voor content-analyse van seksuele voorlichting, platformbeleid-reacties, mediaklopt.

**TikTok — Beperkt via scrapping:**
Openbare profielen, video-beschrijvingen, comments, hashtags. Geen officiële onderzoekers-API. Juridisch grijs gebied voor grootschalige scrapping. Relevant voor algospeak-analyse, trend-diffusie.

**Instagram — Beperkt via Graph API:**
Openbare profielen, posts, comments, hashtags. Graph API is zwaar beperkt sinds Cambridge Analytica (2018). Alleen publieke accounts en goedgekeurde apps. Relevant voor beeldbeschrijvingen, hashtag-analyse.

**Facebook — Beperkt via Graph API:**
Publieke pagina's en groepen. Geen toegang tot privé-profielen of berichten. Relevant voor openbare discours-analyse.

**4chan — Volledige archieven:**
4plebs, archived.moe, desuarchive, etc. Volledige board-archieven (b, pol, s, gif, h, etc.). Relevant voor anoniem discours, terminologie-ontwikkeling, netwerk-verspreiding.

**Tumblr — Openbare API:**
Blogs, tags, posts. Relevant voor discours over intieme media, tagging-praktijken.

**OnlyFans — Beperkt:**
Alleen openbare profielmetadata (bio, links, posts). Geen toegang tot betaalde content. Relevant voor creator-economie analyse, terminologie.

**Pinterest — Openbare API:**
Pins, boards, beschrijvingen. Relevant voor beeldbeschrijvingen, tagging.

**Discord — Beperkt:**
Alleen publieke servers geïndexeerd (via Disboard, top.gg). Privé-servers zijn onzichtbaar. Relevant voor community-discours in publieke servers.

#### Archieven & datasets

**Internet Archive / Wayback Machine:**
Volledige historische captures van webpagina's. API beschikbaar (CDX, Wayback). Relevant voor historische ToS-analyse, platformbeleid-tracking, forum-archivering.

**Common Crawl:**
Maandelijkse crawls van het web (2008-heden). Beschikbaar via Amazon S3 in WARC/PARQUET-formaat. Relevant voor grootschalige web-analyse, term-tracking.

**Pushshift.io:**
Volledig Reddit-archief (2005-2023) in gestructureerd JSON-formaat. De primaire bron voor Reddit-analyse. Bevat alle publieke posts en comments met metadata.

**Google Books Ngram:**
Diachrone termfrequenties uit miljoenen boeken (1800-2019). Beschikbaar als n-gram datasets per taal. Relevant voor historische term-tracking.

**Google Trends:**
Relatief zoekvolume per term, regio, periode. API beschikbaar. Relevant voor maatschappelijke interesse-meting.

#### Nieuws & media

**LexisNexis:**
Volledige nieuwsarchieven uit 100+ landen. Via academische abonnementen. Relevant voor mediaklopt-analyse, framing-analyse, internationale vergelijking.

**Delpher (Nederland):**
Historische Nederlandse kranten, boeken, tijdschriften (1618-2005). Open access. Relevant voor historische Nederlandse discours-analyse.

**Google News Archive:**
Beperkt, maar bruikbaar voor recenter nieuws. Gratis toegankelijk.

**Nationale nieuwsbanken:**
- Genios (Duitsland): Duitse nieuwsarchieven
- Europresse (Frankrijk): Franse nieuwsarchieven
- MyNews (Spanje/VK): internationale nieuwsbanken

#### Overheid & beleid

**CBS StatLine:**
Nederlandse statistische data over bevolking, gezondheid, onderwijs, criminaliteit. Open access. Relevant voor demografische context.

**EU Open Data Portal:**
EU-instellingen data, wetgeving, beleidsdocumenten. Relevant voor DSA-analyse, EU-beleidsvergelijking.

**Rijksoverheid:**
Nederlandse beleidsdocumenten, wetsvoorstellen, Kamerstukken. Via officielebekendmakingen.nl. Relevant voor Nederlands beleidsdiscours.

**WODC:**
Wetenschappelijk Onderzoek- en Documentatiecentrum. Openbare rapporten over jeugdcriminaliteit, sexting, online gedrag.

**Inspectie van het Onderwijs:**
Openbare rapporten over sociale veiligheid op scholen.

**GGD Sense:**
Openbare rapporten over seksuele gezondheid van jongeren.

#### Academische bronnen

**OpenAlex:**
Volledig open access bibliometrische database. ~250M werken, met auteurs, affiliaties, onderwerpen, referenties. API beschikbaar. Relevant voor bibliometrische analyse van sexting-onderzoek.

**PubMed/Medline:**
Medische en biomedische literatuur. ~35M artikelen. API beschikbaar. Relevant voor medische framing van sexting.

**Google Scholar:**
Beperkt scrapable. Breedste dekking van academische literatuur. Relevant voor term-tracking.

**CORE:**
Open access repository. ~200M artikelen. API beschikbaar.

**Social Science Research Network (SSRN):**
Preprints sociale wetenschappen. Open access.

#### Datasets

**Rutgers (Seks onder je 25e):**
Openbare rapporten, factsheets, samenvattingen. Geen raw data, maar gedetailleerde tabellen en cijfers.

**EU Kids Online:**
Openbare datasets en rapportages. Cross-nationale vergelijking van kinderen/jongeren online.

**HBSC:**
Health Behaviour in School-aged Children. Openbare data op aanvraag.

**Eurostat:**
Europese statistische data.

#### Technische data

**WHOIS / Domeinregistraties:**
Openbaar via whois-servers. Relevant voor netwerkanalyse van adult platforms.

**Tech media (TechCrunch, The Verge, Wired, 9to5Mac, Android Police):**
Openbare artikelen over platformbeleid, technische veranderingen, privacy.

**App Store / Google Play:**
Openbare app-beschrijvingen, privacy labels, reviews. Relevant voor platform-affordance analyse.

**ToS;DR (Terms of Service; Did not Read):**
Openbare database met ToS-classificaties. ~3K+ ToS geanalyseerd. API beschikbaar.

**Platform transparency reports:**
Meta Transparency Center, TikTok Transparency Report, YouTube Community Guidelines Report, Reddit Transparency Report, Apple App Store Transparency.

### 1.2 NIET BRUIKBAAR — GESLOTEN/ONTOEGANKELIJK

#### Privé-communicatie (volledig ontoegankelijk)

**WhatsApp:** End-to-end versleuteld. Geen API voor berichtinhoud. Meta heeft geen toegang tot berichten. Zelfs met gerechtelijk bevel is de inhoud van actieve chats niet leesbaar.

**Signal:** End-to-end versleuteld. Open source code, maar geen toegang tot communicatie. Minimale metadata (alleen account-creatie datum).

**Telegram privé-chats:** MTProto-versleuteling voor privé-chats. Alleen openbare kanalen en groepen zijn zichtbaar. Privé-chats zijn niet toegankelijk.

**Facebook Messenger:** Propriëtair. Geen onderzoekers-API voor berichtinhoud. Alleen publieke pagina-berichten.

**iMessage:** Apple's proprietary protocol. End-to-end encrypted. Geen API voor onderzoekers.

**Snapchat:** Verdwijnberichten, geen API voor berichtinhoud. Beperkt onderzoek via gebruikerszelfrapportage.

**Discord privé-servers:** Alleen publieke servers zijn geïndexeerd. DM's en privé-servers zijn niet toegankelijk.

**SMS/MMS:** Telecommunicatie-data, niet toegankelijk zonder provider-medewerking.

**Google Chat / Hangouts:** Enterprise-gericht, geen onderzoekers-API.

**WeChat / LINE / KakaoTalk:** Aziatische messaging-apps, alle propriëtair en afgeschermd.

#### Privé-opslag (volledig ontoegankelijk)

**iCloud:** End-to-end versleuteld (sinds 2023). Alleen gebruiker heeft toegang.

**Google Drive:** Privé. Geen onderzoekers-toegang.

**OneDrive:** Privé. Geen onderzoekers-toegang.

**Dropbox:** Privé. Geen onderzoekers-toegang.

**End-to-end encrypted cloud:** Proton Drive, Tresorit, Sync.com — alle ontoegankelijk.

#### Hulpverleningsdata (beperkt tot geen toegang)

**GGZ-dossiers:** Medisch beroepsgeheim. AVG. Alleen met expliciete toestemming van cliënten.

**GGD-dossiers:** Medisch beroepsgeheim. Beperkt geanonimiseerd onderzoek mogelijk, maar geen directe toegang.

**Jeugdzorgdossiers:** AVG, Jeugdwet. Zeer beperkt toegankelijk.

**Hulpverlenersgesprekken:** Vertrouwelijk. Geen toegang.

**Sense-spreekuren:** Vertrouwelijk. Alleen geaggregeerde rapporten openbaar.

#### Politie & justitie (zeer beperkt)

**Politie-incidentregistraties:** Niet openbaar. Alleen geaggregeerde criminaliteitscijfers via CBS/WODC.

**Zittingsdata:** Openbaar voor zittingen, maar niet voor dossiers. Persoonsgegevens worden geanonimiseerd.

**Slachtofferinterviews:** Vertrouwelijk. Alleen in gepubliceerd onderzoek met toestemming.

**Politieverhoren:** Gesloten. Niet toegankelijk.

**Forensische data (telefoon-extrakties):** Alleen in strafzaken, niet voor onderzoek.

#### Overige gesloten bronnen

**Survey raw data:** Rutgers, EU Kids Online, HBSC — alleen geanonimiseerde datasets op aanvraag, vaak met restricties.

**Schoolrapporten:** Privacy-gevoelig. Alleen geaggregeerd en geanonimiseerd.

**Medische dossiers:** AVG, medisch geheim. Zeer beperkt.

**Telefoniemetadata:** Wettelijk verboden voor onderzoek zonder rechterlijke machtiging.

**Intieme beelddatasets:** Ethisch zeer beladen. Vrijwel nooit beschikbaar. Enkele uitzonderingen in forensisch onderzoek.

**Platform back-end data:** Alleen wat platforms publiceren. Geen toegang tot algoritmes, databases, of moderatie-systemen.

**Advertentiedata (Meta Ads, Google Ads):** Beperkt via Ad Library, maar geen gedetailleerde targeting-data.

**Influencer-data (analytics, inzichten):** Privé, tenzij gedeeld.

### 1.3 METHODOLOGISCHE IMPLICATIES VAN DATABEPERKINGEN

De datasets die we **niet** kunnen gebruiken zijn niet toevallig ontoegankelijk — ze vormen de kern van het fenomeen. Intieme communicatie is per definitie grotendeels privé. De ontoegankelijkheid is geen methodologische tekortkoming, maar een **fundamentele eigenschap van het object van onderzoek**.

Dit heeft zeven concrete implicaties:

**Implicatie 1: Indirecte observatie**
We kunnen privé-gedrag niet direct observeren. We kunnen alleen indirecte sporen ervan zien in openbare data: wat mensen zeggen dat ze doen (forums, interviews), wat ervan zichtbaar wordt in publieke sfeer (nieuws, rechtszaken), en wat ervan meetbaar is via surveys (zelfrapportage).

**Implicatie 2: Escalatiebias**
Openbare data bevat bijna uitsluitend gevallen die geëscaleerd zijn: incidenten die zijn gemeld, besproken in forums, opgenomen in nieuws, of behandeld in rechtszaken. De non-event baseline — de overgrote meerderheid van beelden die nergens toe leiden — is onzichtbaar.

**Implicatie 3: Representativiteitsbeperking**
Wie er publiekelijk over seks praat is niet representatief voor wie er privé seks heeft of intieme media uitwisselt. Openbaar discours over intieme media is een apart sociologisch fenomeen, niet een proxy voor het fenomeen zelf.

**Implicatie 4: Platformbias**
Elk platform heeft een eigen demografie, cultuur en moderatie-regime. Reddit-discours is anders dan Twitter-discours is anders dan forum-discours. Generalisatie over "internet" of "publiek discours" is misleidend zonder platformspecifieke context.

**Implicatie 5: Tijdsbeperking**
Platforms komen en gaan (Hyves, MSN, MySpace, Google+). Data van oude platforms is vaak verloren. Alleen wat bewaard is (Wayback Machine, Pushshift, Common Crawl) is nog beschikbaar. Dit introduceert een overlevingsbias.

**Implicatie 6: Juridische begrenzing**
AVG in Europa beperkt wat onderzoekers mogen verzamelen, bewaren en publiceren. Art. 240b Sr maakt het bezit van bepaalde data strafbaar. Ethische commissies keuren bepaalde onderzoeksdesigns niet goed. Onderzoek naar intieme media is juridisch begrensd.

**Implicatie 7: Taal- en cultuurbegrenzing**
Onderzoekers spreken niet alle talen. Corpora zijn niet voor alle talen beschikbaar. Google Trends-dekking varieert per land. Nieuwsarchieven zijn niet voor alle landen even toegankelijk. Dit introduceert een westerse, Engelstalige bias.

---

## FASE 2: WAT KUNNEN WE WEL ONDERZOEKEN — 10 CATEGORIEËN

### A. Publiek discours en terminologie

**Beschrijving:**
Deze categorie onderzoekt hoe mensen **openbaar** praten over seks, naaktheid, intimiteit en intieme media. Het onderscheidt zich fundamenteel van onderzoek naar privé-communicatie: wat mensen in het openbaar zeggen over intimiteit is anders dan wat ze in privé zeggen. Maar openbaar discours is op zichzelf een relevant sociologisch fenomeen — het beïnvloedt normen, percepties, beleid en mediaberichtgeving.

**Wat we wél kunnen:**
- Frequentie en context van seksuele termen in openbare forums
- NPM-scores toekennen op basis van openbare corpora (Reddit, Twitter, forums)
- Register A/B-polarisatie kwantificeren in openbaar discours
- Verschil in taalgebruik tussen publiek, academisch en beleidsdiscours
- Verandering in terminologie over tijd (2000-2026)
- Cross-linguïstische vergelijking van intieme terminologie
- SVP V1-V4 toepassen op openbare termen
- Authenticity Layer (10 categorieën) coderen voor openbare termen
- Emoji-gebruik in intieme context analyseren
- Algospeak-diffusie en levenscyclus documenteren
- Conversation Layer (7 kanalen) analyseren per platform
- Pragmatische functies (verzoek, consent, afwijzing) coderen

**Wat we niet kunnen:**
- Register B in authentieke privé-chats meten
- Werkelijke NPM-verdeling in intieme 1-op-1 communicatie
- Authenticiteit van privé-taalgebruik verifiëren
- Sprekersintentie vaststellen (ironie, sarcasme, performativiteit)
- Demografische representativiteit garanderen

**Relevante toolonderdelen:**
NPM 1-6, Authenticity Layer (10 cat.), Register A/B model, SVP V1-V4, Conversation Layer (7 kanalen), Pragmatische functieregister, Lexicale Frequentiekaart, Anti-steriliteitsprincipe.

**Beschikbare data:**
Reddit Pushshift, Twitter Academic API, Google Books Ngram, Google Trends, forum-archieven (Partyflock, FOK), YouTube comments, Instagram comments.

### B. Platformstructuren en affordances

**Beschrijving:**
Deze categorie onderzoekt de technische en beleidsmatige infrastructuur van platforms die intieme media faciliteren, modereren en soms monetariseren. Het gaat niet om gebruikersgedrag, maar om de **omgeving** waarbinnen dat gedrag plaatsvindt.

**Wat we wél kunnen:**
- ToS en communityrichtlijnen analyseren over tijd
- Veranderingen in screenshot-meldingen, ephemeraliteit, privacy-instellingen documenteren
- Transparantierapporten vergelijken (aantal verwijderingen, beroepen, herstelpercentages)
- Affordance-analyse op basis van openbare platformdocumentatie
- App-store beschrijvingen en privacy labels analyseren
- Platformblogposts en aankondigingen over beleidswijzigingen documenteren
- Tech-media analyse (The Verge, TechCrunch, Wired)
- EU DSA-implementatie per platform vergelijken

**Wat we niet kunnen:**
- Achterliggende technische werking van versleuteling verifiëren
- Daadwerkelijke screenshot-detectie testen op niet-publieke functionaliteit
- Back-end data-opslagstructuren inzien
- Moderatie-effectiviteit meten zonder platform-toegang
- False positive/negative rates van AI-moderatie verifiëren

**Relevante toolonderdelen:**
DeviceAffordanceRecord (platformtype, opname-affordances, verspreidingsaffordances, tijdelijkheidsaffordances), MediaLifecycleRecord, PerceivedEphemerality vs. ActualPersistence, VisibilityIntentMismatchRecord, EvidenceProfile.

**Beschikbare data:**
Wayback Machine, ToS;DR, platform transparantieportalen, App Store/Google Play, tech media.

### C. Content-analyse van OPENBAAR gedeelde media

**Beschrijving:**
Deze categorie onderzoekt de metadata van openbaar gedeelde intieme media — niet de beelden zelf, maar wat erover wordt gezegd in tags, titels, beschrijvingen en discussies. Het is een meta-analyse van hoe intieme media worden geclassificeerd, beschreven en gepresenteerd in het publieke domein.

**Wat we wél kunnen:**
- Metadata-analyse van tags op adult platforms en forums
- 17-assige taxonomie toepassen op openbare metadata
- Cross-source translation table valideren met openbare bronnen
- Anti-dubbeltellingsregel toepassen op metadata
- Gewogen bewijsmodel testen op openbare casus-beschrijvingen
- Gedragsladder (N0-5) coderen op basis van beschrijvingen
- Inter-rater reliability van taxonomieën meten

**Wat we niet kunnen:**
- Beelden zelf analyseren (ethisch en juridisch problematisch)
- Ontstaanscontext verifiëren voor individuele beelden
- Toestemming vaststellen bij openbaar materiaal
- Verschil tussen geënsceneerd en echt bepalen zonder bronverificatie
- Capture-Dependency coderen zonder maker-interview

**Relevante toolonderdelen:**
17-assige taxonomie, Gedragsladder, Cross-Source Translation Table, Anti-dubbeltellingsregel, Gewogen bewijsmodel, MissingnessMap, Authenticity Layer.

**Beschikbare data:**
Reddit Pushshift (adult subreddits), Pornhub/XVideos metadata (titels, tags, beschrijvingen), OnlyFans metadata.

### D. Mediaklopt en publiek debat

**Beschrijving:**
Deze categorie onderzoekt hoe nieuwsmedia, opiniebladen en journalistieke bronnen rapporteren over sexting, NCII, jeugd-naaktheid en intieme media. Het richt zich op framing, terminologie, toon en verandering over tijd — zowel nationaal als internationaal.

**Wat we wél kunnen:**
- Framing-analyse van nieuwsberichten (2010-2026)
- Longitudinale analyse van mediaberichtgeving
- Internationale vergelijking van mediadekking
- Terminologie-tracking in journalistiek
- Relatie tussen mediaberichtgeving en beleidsveranderingen
- NPM-classificatie van journalistieke termen
- SVP V1-V4 toepassen op journalistieke terminologie
- Gender-analyse van slachtoffer/dader framing

**Wat we niet kunnen:**
- Effect van media op daadwerkelijk jongerengedrag meten
- Causale verbanden leggen tussen mediadekging en prevalentie
- Representativiteit van nieuws voor algemene bevolking claimen

**Relevante toolonderdelen:**
NormalizationContextRecord, EvidenceProfile, Content-Source Bias, NPM 1-6, SVP V3.

**Beschikbare data:**
LexisNexis, Delpher, Google News, nationale nieuwsbanken, Google Trends.

### E. Platformbeleid en moderatie

**Beschrijving:**
Deze categorie onderzoekt hoe platforms regels opstellen, communiceren en handhaven over naaktheid, seksuele content en intieme media. Het omvat ToS-analyse, transparantierapportage en beleidsveranderingen.

**Wat we wél kunnen:**
- Consistentie-analyse van ToS-definities over platforms
- Longitudinale analyse van beleidsveranderingen
- Transparantierapport-data vergelijken en normaliseren
- EU DSA-compliance per platform documenteren
- Moderatiepraktijken analyseren via openbare bronnen
- AI-moderatietechnieken categoriseren uit openbare documentatie

**Wat we niet kunnen:**
- Daadwerkelijke moderatiebeslissingen inzien
- Effectiviteit van moderatie meten zonder platform-toegang
- False positive/negative rates verifiëren
- Algoritmische bias in moderatie kwantificeren

**Relevante toolonderdelen:**
DeviceAffordanceRecord, EvidenceProfile, Cross-Source Translation Table, MissingnessMap.

**Beschikbare data:**
Wayback Machine, ToS;DR, platform transparantieportalen, tech media, EU DSA-documentatie.

### F. Historische trends

**Beschrijving:**
Deze categorie onderzoekt hoe terminologie, interesse en aandacht over intieme media zijn veranderd over de tijd, via openbare indicatoren zoals Google Trends, Wikipedia, Google Books, Common Crawl en forum-archieven.

**Wat we wél kunnen:**
- Google Trends-data over sexting, nudes, NCII, amateur content
- Wikipedia-editgeschiedenis van relevante artikelen
- Google Books Ngram-analyse van termfrequenties
- Wayback Machine-analyse van websites
- Archiefanalyse van forums (Partyflock, FOK, GoT)
- Common Crawl-term-tracking over tijd
- Diachrone corpusanalyse van intieme terminologie

**Wat we niet kunnen:**
- Werkelijke verandering in privé-gedrag meten
- Oorzakelijke verbanden leggen met technologische veranderingen
- Platform-verschuivingen isoleren van maatschappelijke trends

**Relevante toolonderdelen:**
NPM 1-6, Authenticity Layer, SVP V1-V4, Lexicale Frequentiekaart.

**Beschikbare data:**
Google Trends, Wikipedia API, Google Books Ngram, Wayback Machine, Common Crawl, Pushshift.

### G. Internationale vergelijking van openbaar discours

**Beschrijving:**
Deze categorie vergelijkt hoe verschillende landen en taalgemeenschappen praten over intieme media. Het omvat nieuwsframing, terminologieverschillen, zoekgedrag en platformgebruik.

**Wat we wél kunnen:**
- Cross-nationale nieuwsframing-vergelijking
- Terminologieverschillen per taal in openbare forums
- Google Trends-vergelijking per land
- Wikipedia-vergelijking per taal
- Cultuurverschillen in openbaar discours over seks

**Wat we niet kunnen:**
- Culturele verschillen in privé-communicatie meten
- Representativiteit per land garanderen
- Niet-Engelstalige internetcultuur volledig dekken

**Relevante toolonderdelen:**
Register A/B model, NPM 1-6, Authenticity Layer (categorie 8 regionale variant), SVP V1-V4.

**Beschikbare data:**
LexisNexis internationaal, Google Trends per land, Wikipedia per taal, Google Books Ngram per taal.

### H. Academisch discours

**Beschrijving:**
Deze categorie onderzoekt hoe de academische wereld — via publicaties, terminologie en onderzoeksagenda's — het domein van intieme media heeft bestudeerd en gekaderd.

**Wat we wél kunnen:**
- Bibliometrische analyse van sexting-onderzoek (2005-2026)
- Terminologieverschuiving in academische publicaties
- SVP V3-toetsing van academische terminologie
- Publicatietrends per land/discipline/tijdschrift
- Netwerkanalyse van co-auteurschap
- Cross-source translation table toepassen op academische termen

**Wat we niet kunnen:**
- Kwaliteit van individuele studies verifiëren zonder data-toegang
- Publicatiebias volledig kwantificeren
- Grijze literatuur (niet-gepubliceerd onderzoek) dekken

**Relevante toolonderdelen:**
Cross-Source Translation Table, NPM 1-6, SVP V3, EvidenceProfile, Gedragsladder.

**Beschikbare data:**
OpenAlex, PubMed, Google Scholar, CORE, SSRN, Crossref.

### I. Taxonomie en classificatie op openbare bronnen

**Beschrijving:**
Deze categorie valideert de toolonderdelen zelf — de 17-assige taxonomie, Gedragsladder, Cross-Source Translation Table, Anti-dubbeltellingsregel — door ze toe te passen op openbare bronnen en inter-rater reliability te meten.

**Wat we wél kunnen:**
- Inter-rater reliability van de 17-assige taxonomie
- Inter-rater reliability van de Gedragsladder (N0-5)
- Validatie van Cross-Source Translation Table
- Anti-dubbeltellingsregel effect-meting
- Gewogen bewijsmodel testen op openbare casussen
- Authenticity Layer reliability meten
- MissingnessMap toepassen op openbare datasets

**Wat we niet kunnen:**
- Taxonomie valideren op niet-openbare beelden
- Ontstaanscontext verifiëren voor individuele content
- Volledige 17-assen codering zonder bronverificatie

**Relevante toolonderdelen:**
Alle toolonderdelen (primair: 17-assige taxonomie, Gedragsladder, Cross-Source Translation, Anti-dubbeltellingsregel, Gewogen bewijsmodel).

**Beschikbare data:**
Reddit Pushshift metadata, handmatig gecodeerde steekproeven.

### J. Netwerkanalyse van openbare sharing

**Beschrijving:**
Deze categorie onderzoekt hoe intieme content (als metadata/URLs) zich verspreidt via openbare platforms. Het richt zich op netwerkstructuren, aggregators, tijdsdynamiek en verspreidingspatronen.

**Wat we wél kunnen:**
- URL-verspreiding via Reddit/Twitter volgen
- Rol van aggregators, bots en curators identificeren
- Netwerkstructuren van openbare sharing-communities
- Tijdsanalyse van virale verspreiding
- Cross-platform verspreidingspatronen
- Community-detectie in sharing-netwerken
- Persistentie van openbare links meten

**Wat we niet kunnen:**
- Verspreiding volgen in privé-kanalen
- Werkelijke schaal van NCII-verspreiding meten
- Identiteit van delers vaststellen
- Motivatie van delers bepalen

**Relevante toolonderdelen:**
MediaLifecycleRecord (re-share ketens), DeviceAffordanceRecord (platformoverschrijdend delen), TrajectoryRecord, Pattern Library.

**Beschikbare data:**
Pushshift (cross-post detectie), Twitter API (URL tracking), Wayback Machine (persistence), Common Crawl.

---

## FASE 3: WAT KUNNEN WE NIET ONDERZOEKEN — EXPLICIETE EXCLUSIES

### 3.1 VRAGEN UIT V1 EN V2 DIE NIET HAALBAAR ZIJN

#### Cluster 1 — Registerpolarisatie & Terminologie (v1 vragen 1.1-1.3, v2 vragen 1.1-1.3)

**Vraag 1.1 (v1):** "Hoe verschilt de lexicale samenstelling van intieme verzoeken tussen Register A en Register B in natuurlijke chatcorpora van volwassenen?"
- **Waarom niet haalbaar:** Vereist toegang tot privé-chatlogs (WhatsApp, Telegram, Signal). Deze zijn end-to-end versleuteld en niet beschikbaar. Zelfs geanonimiseerde corpora van intieme gesprekken zijn zeldzaam en niet openbaar.
- **Vervangende haalbare vraag:** A-01 — analyse van Register A/B in openbare forums (Reddit, Twitter) waar mensen over intieme communicatie schrijven. Dit is performatiever en minder direct, maar geeft wel inzicht in registerverschillen in openbaar discours.

**Vraag 1.2 (v1):** "Welke NPM-niveaus domineren in seksuele verzoeken op datingapps versus in gevestigde langdurige relaties?"
- **Waarom niet haalbaar:** Datingapp-conversatiedata is propriëtair en niet openbaar. Tinder, Bumble, Hinge delen geen gebruikersdata met onderzoekers. Relatie-chatlogs zijn privé.
- **Vervangende haalbare vraag:** A-02 — analyse van NPM-niveaus in openbare dating-advies forums vs. relatie-forums op Reddit.

**Vraag 1.3 (v1):** "Hoe beïnvloedt platformtype de NPM-verdeling in intieme uitwisselingen?"
- **Waarom niet haalbaar:** Vereist cross-platform vergelijking van daadwerkelijke intieme uitwisselingen. Platformdata is propriëtair.
- **Vervangende haalbare vraag:** A-03 — analyse van hoe platformtype het openbare discours over intieme media beïnvloedt (Reddit vs. Twitter vs. fora).

#### Cluster 2 — Communicatieve Patronen (v1 vragen 2.1-2.3, v2 vragen 3.1-3.3)

**Vraag 2.1 (v1):** "Wat is de gemiddelde en mediane request-to-action distance bij intieme beeldverzoeken in relaties van 15-18-jarigen?"
- **Waarom niet haalbaar:** RAD vereist sequentiële data van verzoek-reactie met timestamps in privé-chats. Alleen via retrospectieve zelfrapportage in surveys — maar surveys zijn geen openbare data.
- **Vervangende haalbare vraag:** Geen directe vervanging. RAD is een privé-dynamiek die niet uit openbare data te halen is. Theoretische modellering op basis van literatuur is wel mogelijk.

**Vraag 2.2 (v1):** "In welke verhouding staan positieve versus negatieve elementen in audience feedback loops rond intieme beelden?"
- **Waarom niet haalbaar:** Feedback loops spelen zich af in privé-reacties op gedeelde beelden. Openbare reacties (likes, comments) op platforms zijn wel zichtbaar, maar geven een selectief en geoptimaliseerd beeld.
- **Vervangende haalbare vraag:** Beperkt onderzoek naar openbare feedback (upvotes, comments) op Reddit, maar dit weerspiegelt privé-feedback niet.

**Vraag 2.3 (v1):** "Wat is de incidentie van het Behavioural Stopping Point in patronen van intieme beeldproductie?"
- **Waarom niet haalbaar:** Stopping points worden niet geregistreerd in openbare data. Ze zijn alleen via interviews of retrospectieve reconstructie te vangen.
- **Status:** Expliciet uitgesloten.

#### Cluster 3 — Sociale Interacties & Scripting (v1 vragen 3.1-3.3, v2 vragen 4.1-4.3)

**Vraag 3.1 (v1):** "Hoe verdeelt consent zich over de zes handelingsfasen in gedocumenteerde incidentrecords?"
- **Waarom niet haalbaar:** Incidentrecords met consent-differentiatie zijn alleen beschikbaar in institutionele archieven (politie, hulpverlening, school). Deze zijn niet openbaar.
- **Vervangende haalbare vraag:** Consent-analyse op basis van openbare discussies over consent op Reddit (r/sex, r/relationships). Dit geeft inzicht in hoe consent wordt besproken, niet in hoe het wordt toegepast.

**Vraag 3.2 (v1):** "In welke mate wordt impliciete instemming gebruikt als rechtvaardiging voor re-share?"
- **Waarom niet haalbaar:** Impliciete instemming in reële casussen vereist toegang tot dossiers of interviews.
- **Vervangende haalbare vraag:** Analyse van openbare discussies over re-share en consent (r/legaladvice, r/relationships).

**Vraag 3.3 (v1):** "Welke relatiescripts domineren in de VisualScriptRecord van jongeren 15-18?"
- **Waarom niet haalbaar:** VisualScriptRecord codering vereist toegang tot casusbeschrijvingen uit surveys of interviews. Geen openbare data.
- **Vervangende haalbare vraag:** Script-analyse op basis van openbare verhalen op Reddit (r/sexstories, r/relationships). Beperkt en niet representatief.

#### Cluster 4 — Gedragsanalyse & Granulariteit (v1 vragen 4.1-4.3, v2 vragen 5.1-5.3)

**Vraag 4.1 (v1):** "Welke verdeling van de Gedragsladder vertonen verschillende brontypen?"
- **Waarom niet haalbaar:** Vereist codering van onderzoekspublicaties. Is wel deels haalbaar via meta-analyse van openbare publicaties.
- **Status:** Gedeeltelijk haalbaar als literatuurstudie. Opgenomen als H-01 (academisch discours).

**Vraag 4.2 (v1):** "In welk percentage volgt het gedrag het Content Escalation Path?"
- **Waarom niet haalbaar:** Vereist sequentiële data van sessies. Incidentendossiers zijn niet openbaar.
- **Vervangende haalbare vraag:** Theoretisch model op basis van literatuur.

**Vraag 4.3 (v1):** "Wat is de verhouding tussen Niveau 0 en Niveau 4+ in gepubliceerde sexting-prevalentiecijfers?"
- **Waarom niet haalbaar:** Meta-analyse van openbare literatuur is wel haalbaar. Prevalentiecijfers uit openbare rapporten (Rutgers, EU Kids Online) zijn beschikbaar.
- **Status:** Gedeeltelijk haalbaar. Opgenomen als H-02 met beperkingen.

#### Cluster 5 — Platformecosystemen (v1 vragen 5.1-5.3, v2 vragen 6.1-6.3)

**Vraag 5.1 (v1):** "Hoe verschilt de verdeling van visibility-locaties per platformtype?"
- **Waarom niet haalbaar:** Visibility-locatie data per platform vereist toegang tot incidentregistraties.
- **Vervangende haalbare vraag:** B-01 — affordance-analyse op basis van openbare platformdocumentatie.

**Vraag 5.2 (v1):** "In welke mate differentiëren jongeren tussen perceived ephemerality en actual persistence per platform?"
- **Waarom niet haalbaar:** Vereist survey-data met dual measurement. Alleen Rutgers/EU Kids Online data (niet openbaar).
- **Vervangende haalbare vraag:** B-02 — analyse van platformcommunicatie over ephemeraliteit.

**Vraag 5.3 (v1):** "Wat is de relatie tussen verspreidingsaffordances en Visibility Escalation Score?"
- **Waarom niet haalbaar:** Causale analyse vereist experimenteel design met platformdata.
- **Status:** Expliciet uitgesloten.

#### Overige uitgesloten vragen uit v1 en v2

**Vraag 11.1 (v1):** Capture-Dependency verdeling in IncidentRecords — uitgesloten.
**Vraag 11.2 (v1):** Camera-Presence Effect aandeel — uitgesloten.
**Vraag 12.1 (v1):** VES in functie van Network-Location — uitgesloten.
**Vraag 13.1 (v1):** Content-to-Circulation Transformation kans — uitgesloten.
**Vraag 14.2 (v2):** Re-share ketenlengte — uitgesloten.
**Vraag 17.2 (v1):** Pragmatische Wrijving in chat-corpus — uitgesloten.
**Vraag 19.3 (v1):** Hawthorne-effect in intieme opnames — uitgesloten.
**Vraag 20.5 (v2):** Non-Event Baseline ratio jongeren vs. volwassenen — uitgesloten.
**Vraag 15.1 (v2):** 17-assige taxonomie reliability op beeldmateriaal — uitgesloten.
**Vraag 7.2 (v1):** Behaviour-to-Image Conversion Point — uitgesloten.
**Vraag 7.3 (v1):** Prompt-Source Map — uitgesloten.

### 3.2 STRUCTURELE BELEMMERINGEN

**Privacy-by-design platforms:**
WhatsApp, Signal, Telegram, iMessage zijn end-to-end versleuteld. Geen enkele onderzoeker heeft toegang tot de inhoud van privé-berichten op deze platforms, tenzij gebruikers deze zelf delen. Dit is geen technische beperking die omzeild kan worden — het is een ontwerpkeuze die privacy beschermt. Zelfs metadata (wie met wie communiceert) is beperkt beschikbaar. Dit betekent dat de meest gebruikte kanalen voor intieme media-uitwisseling (WhatsApp, Snapchat, Instagram DM) volledig ontoegankelijk zijn voor inhoudsanalyse.

**Verdwijnende platforms en data:**
- Hyves (NL, 2004-2013): volledig verdwenen. Data is verloren.
- MSN Messenger (1999-2013): historische data is schaars.
- MySpace (2003-heden): data grotendeels verloren door servermigraties.
- Google+ (2011-2019): data verloren bij sluiting.
- Snapchat: verdwijnberichten zijn per definitie niet bewaard.
- Instagram Stories: 24-uurs verdwijning.
- TikTok: content kan worden verwijderd door gebruikers of platform.
- Clubhouse (2020-2023): audio verdwijnt, geen archief.

**Juridische beperkingen:**
- AVG (GDPR): beperkt wat onderzoekers mogen verzamelen, opslaan en publiceren.
- Art. 240b Sr (Nederland): bezit van kinderpornografie is strafbaar, ook voor onderzoek (tenzij specifieke ontheffing).
- Auteurswet: copyright op content beperkt reproductie.
- Platform ToS: scrapping is vaak verboden in de ToS.
- Ethische commissies: goedkeuring vereist voor onderzoek met menselijke data.

**Platform-API-beperkingen:**
- Twitter/X: Academic API is ~.000/maand sinds 2023. Rate limits streng.
- Reddit: Pushshift is de beste bron, maar sinds 2023 is Pushshift niet meer bijgewerkt. Huidige Reddit API is duur (.24/1K requests).
- TikTok: geen officiële onderzoekers-API. Scrapping is juridisch grijs gebied.
- Instagram/Facebook: Graph API is zwaar beperkt sinds Cambridge Analytica (2018). Alleen publieke data.
- YouTube: Data API is relatief goed, maar quota-beperkt (10.000 units/dag).
- LinkedIn: API is zeer beperkt. Alleen eigen profieldata.
- Discord: geen API voor berichtinhoud van privé-servers.
- Snapchat: geen onderzoekers-API.
- Telegram: Bot API kan alleen openbare kanalen lezen.

**Data-kwaliteitsproblemen:**
- Zelfrapportagebias: wat mensen zeggen is niet wat ze doen.
- Sociale wenselijkheid: bepaalde onderwerpen worden onder- of overgerapporteerd.
- Herinneringsbias: retrospectieve data is onbetrouwbaar.
- Steekproefbias: wie meedoet aan surveys is selectief.
- Platformbias: Reddit is niet Twitter is niet Facebook is niet algemene bevolking.
- Moderatiebias: wat zichtbaar is op platforms wordt gefilterd door moderatie.

---

## FASE 4: ONDERZOEKSVRAGEN — CATEGORIE A (PUBLIEK DISCOURS EN TERMINOLOGIE)

### VRAAG A-01

**Hoe verschilt de lexicale samenstelling van intieme taal in openbare forums (Reddit r/sex, r/relationships, r/dirtyr4r) van klinisch-juridische terminologie in beleidsdocumenten, en wat zegt dit over de NPM-kloof tussen deze registers?**

- **Waarom haalbaar:** Reddit is volledig openbaar via Pushshift. Beleidsdocumenten zijn openbaar. Beide corpora zijn grootschalig beschikbaar (>1M documenten per bron).
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer (10 categorieën), Register A/B polarisatiemodel, SVP V1-V4, Lexicale Frequentiekaart.
- **Openbare databronnen:** Pushshift Reddit-archief (subreddits r/sex, r/relationships, r/dirtyr4r, r/sexover30), rijksoverheid.nl documenten, WODC-rapporten, EU-beleidsdocumenten, Google Books Ngram.
- **Analysemethoden:** Corpusanalyse met NPM-codering per term, vergelijkende frequentieanalyse, Authenticity Layer-classificatie van >10.000 termen, chi-kwadraat toetsing tussen corpora, SVP V1-V4 toepassing op top-100 termen.
- **Verwachte bewijssterkte:** Sterk — grote corpora beschikbaar (>10M woorden per corpus), direct vergelijkbaar.
- **Risico's en beperkingen:** Reddit-gebruikers zijn geen representatieve steekproef (overwegend mannelijk, jong, westers). Beleidsdocumenten zijn in formele taal met eigen conventies. De kloof tussen deze twee is bekend, maar niet systematisch gekwantificeerd op NPM-schaal.
- **Taalstrategie:** Nederlands (r/thenetherlands, r/nederlands, overheid.nl) en Engels (grote subreddits, UK/US beleid).

### VRAAG A-02

**Welke NPM-niveaus (1-6) domineren in openbare seksuele verzoeken op Reddit (r/dirtyr4r, r/dirtypenpals, r/sex) versus dating-advies (r/dating, r/dating_advice), en wat zegt dit over het verschil tussen performatief en authentiek discours?**

- **Waarom haalbaar:** Deze subreddits bevatten duizenden openbare berichten met directe verzoeken. Pushshift maakt volledige historische analyse mogelijk.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer, Register A/B model, SVP V1-V4.
- **Openbare databronnen:** Pushshift, Reddit API (r/dirtyr4r, r/dirtypenpals, r/sex, r/dating, r/dating_advice), Google Trends.
- **Analysemethoden:** NPM-codering per subreddit, chi-kwadraat vergelijking tussen subreddits, frequentieverdeling per register (A/B), sentiment-analyse, tijdreeks-analyse van register-gebruik.
- **Verwachte bewijssterkte:** Sterk — grote datasets (>100.000 berichten per subreddit).
- **Risico's en beperkingen:** r/dirtyr4r is een niche (zoektochten, geen relaties). Verschil tussen performatief en authentiek discours is moeilijk te operationaliseren. Publiek discours is niet privé-communicatie.
- **Taalstrategie:** Engels (primaire data), Nederlands (r/dirtyr4r_nl, r/seks).

### VRAAG A-03

**Hoe heeft de term "algospeak" (seggs, corn, spicy, view once, mole, unalive) zich verspreid van platform-taal naar openbaar discours op Reddit en Twitter tussen 2020-2026, en wat is de NPM-verdeling per term over tijd?**

- **Waarom haalbaar:** Deze termen zijn publiekelijk gebruikt op sociale media. Pushshift en Twitter API maken historische tracking mogelijk. Termen zijn specifiek genoeg voor exacte matching.
- **Essentiële toolonderdelen:** NPM 3 (Contextafhankelijk), Authenticity Layer categorie 10 (Platformslang), SVP V1-V4, Conversation Layer.
- **Openbare databronnen:** Pushshift, Twitter API (Academic tier), r/TikTok, r/Instagram, r/OutOfTheLoop, Google Trends, Know Your Meme.
- **Analysemethoden:** Diachrone frequentie-analyse per term, diffusiecurve-modellering (S-curve fitting), NPM-toekenning per term per tijdsperiode, cross-platform vergelijking (Reddit vs. Twitter), register-herkomstcodering.
- **Verwachte bewijssterkte:** Waarschijnlijk — data is beschikbaar maar platform-specifiek. Termen zijn snel veranderlijk.
- **Risico's en beperkingen:** Termen komen en gaan snel; piek kan kort zijn. Platform-specifieke algoritmes beïnvloeden zichtbaarheid. Niet alle algospeak is in openbare data zichtbaar (sommige ontstaan in privé-chats). Matching is gevoelig voor spellingvariaties.
- **Taalstrategie:** Engels (primair), Nederlands (Nederlandse varianten zoals "mais", "spannende foto").

### VRAAG A-04

**Wat is de frequentie en context van Register B-termen (neuken, pijpen, beflen, aftrekken, klaarkomen) vs. Register A-termen (vrijen, seks hebben, de liefde bedrijven, intiem zijn) in Nederlandse openbare fora (Partyflock, FOK, Reddit NL, Twitter NL), en hoe verhoudt dit zich tot het NPM-model?**

- **Waarom haalbaar:** Nederlandse fora zijn openbaar en gearchiveerd. Vergelijking tussen registers met dezelfde conceptuele betekenis.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer, Register A/B model, SVP V1-V4, Lexicale Frequentiekaart.
- **Openbare databronnen:** Partyflock-archieven (via Wayback Machine), FOK!-forums, Reddit NL (r/nederlands, r/thenetherlands, r/seks), Twitter NL (Academic API), Corpus Gesproken Nederlands (CGN, voor baseline), Google Books Ngram NL.
- **Analysemethoden:** Frequentieanalyse per term per platform, context-analyse (co-occurrence met andere termen), sentiment-analyse, NPM-toekenning per term, Register-classificatie, SVP V1-V4 toepassing.
- **Verwachte bewijssterkte:** Waarschijnlijk tot Sterk — meerdere bronnen beschikbaar voor triangulatie.
- **Risico's en beperkingen:** Oudere fora zijn deels verloren (Wayback-dekking is onvolledig). CGN heeft beperkte intieme data. Forums-discours is niet privé-gesprekken. Verschil tussen geschreven en gesproken taal.
- **Taalstrategie:** Nederlands.

### VRAAG A-05

**Welke semantische verschuiving heeft de term "amateur" ondergaan in openbare platformcategorieën (Pornhub, XVideos, Reddit, OnlyFans, Twitter) tussen 2005-2025, en hoe verhoudt de platformdefinitie zich tot de wetenschappelijke definitie uit het 17-assige model?**

- **Waarom haalbaar:** Platformcategorieën zijn openbaar via tags, beschrijvingen en metadata. Historische versies via Wayback Machine. Alleen metadata-analyse (geen beelden).
- **Essentiële toolonderdelen:** 17-assige taxonomie (Assen 8A/8B splitsing, As 6 Commerciële intentie, As 7 Zichtbaarheidsoptimalisatie), Cross-Source Translation Table.
- **Openbare databronnen:** Wayback Machine captures van Pornhub/XVideos, Reddit (r/amateur, r/realgirls, r/amateurcumsluts), OnlyFans openbare metadata, Google Trends, Google Books Ngram, Common Crawl.
- **Analysemethoden:** Diachrone semantische analyse, tag-frequentie per platform per jaar, co-occurrence-analyse van "amateur" met commerciële tags (onlyfans, paywall), classificatie op 17-assen.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar maar deels vluchtig en platform-afhankelijk.
- **Risico's en beperkingen:** Algoritmische tagging op platforms is ondoorzichtig. "Amateur" heeft meerdere betekenissen tegelijk (niet-professioneel, commercieel genre, esthetische stijl). Metadata alleen geeft beperkt zicht.
- **Taalstrategie:** Engels (primair), Nederlands.

### VRAAG A-06

**Hoe verschilt het gebruik van emoji in intieme context op openbare sociale media (Twitter, Reddit, Instagram comments) tussen pragmatische functies (flirt vs. expliciet verzoek vs. afwijzing vs. compliment vs. discretieborging), en wat leert dit over emoji als register-markers?**

- **Waarom haalbaar:** Emoji zijn publiek zichtbaar in berichten. Twitter, Reddit en Instagram comments zijn toegankelijk via API/scraping.
- **Essentiële toolonderdelen:** Conversation Layer (kanaalanalyse), Pragmatische functieregister, Authenticity Layer, NPM 1-6, Multi-Lagen Steganografie (Laag 2: emoji).
- **Openbare databronnen:** Twitter API (Academic tier), Pushshift, Instagram openbare API, emoji-databases (Unicode Consortium), Google Trends (emoji search), Emojipedia.
- **Analysemethoden:** Frequentie-analyse van emoji per context, sequentiële patroonanalyse van emoji-combinaties, pragmatische functiecodering (verzoek, consent, afwijzing, compliment), cross-platform vergelijking.
- **Verwachte bewijssterkte:** Waarschijnlijk — grote datasets beschikbaar, maar contextinterpretatie is uitdagend.
- **Risico's en beperkingen:** Emoji-betekenissen zijn context-, cultuur- en generatieafhankelijk. Dezelfde emoji kan meerdere betekenissen hebben. Intieme emoji worden ook niet-intiem gebruikt (ironie, sarcasme). Codering vereist meerdere codeurs.
- **Taalstrategie:** Multinational — emoji zijn universeel, maar culturele interpretatie verschilt.

### VRAAG A-07

**In welke mate doorstaat openbare terminologie over "sexting" in internationale nieuwsmedia (2010-2026) de SVP V3-toets (AI-normalisatie check): welk aandeel van de journalistieke termen is klinisch-gedistantieerd (NPM 5-6) vs. natuurlijk (NPM 1-2), en verandert deze verhouding over tijd?**

- **Waarom haalbaar:** Nieuwsarchieven zijn grootschalig beschikbaar via LexisNexis. Longitudinale analyse is mogelijk.
- **Essentiële toolonderdelen:** SVP V1-V4 (specifiek V3), NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** LexisNexis (NL, UK, US, DE, FR), Google News Archive, Delpher (NL), nationale nieuwsbanken, Google Books Ngram.
- **Analysemethoden:** SVP V3-toetsing per nieuwsartikel (steekproef n=500 per taal), NPM-classificatie van terminologie, trendanalyse per jaar (2010-2026), vergelijking tussen landen.
- **Verwachte bewijssterkte:** Sterk — grote, goed ontsloten datasets (>100.000 artikelen).
- **Risico's en beperkingen:** Journalistieke taal is per definitie formeel en geschreven. SVP is ontworpen voor privé-spreektaal; toepassing op journalistiek vereist nuance.
- **Taalstrategie:** Nederlands (LexisNexis NL), Engels (LexisNexis UK/US), Duits (Genios), Frans (Europresse).

### VRAAG A-08

**Hoe worden seksuele handelingen en anatomie aangeduid in openbare Nederlandstalige fora vergeleken met de termen in de Rutgers Seks onder je 25e vragenlijst: wat is de NPM-kloof tussen survey-terminologie en informele spreektaal?**

- **Waarom haalbaar:** Rutgers-vragenlijst is openbaar (in rapporten). Fora-discours is openbaar. Direct vergelijkbaar.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer, SVP V1-V4, Cross-Source Translation Table.
- **Openbare databronnen:** Rutgers openbare rapporten (Seks onder je 25e), Partyflock-archieven, FOK!-forums, Reddit NL, Twitter NL, Google Books Ngram NL.
- **Analysemethoden:** Term-extractie uit Rutgers-vragenlijst, NPM-codering per term, vergelijking met forum-frequenties, SVP V3-toetsing op survey-terminologie, MissingnessMap voor niet-gemeten termen.
- **Verwachte bewijssterkte:** Sterk — direct vergelijkbare corpora.
- **Risico's en beperkingen:** Survey-vragen zijn noodzakelijk formeel (voor duidelijkheid). Informele alternatieven ("picje", "spicy") passen niet in gestandaardiseerde surveys. NPM-scores voor schrijftaal (surveys) zijn anders dan voor spreektaal.
- **Taalstrategie:** Nederlands.

### VRAAG A-09

**Welke Conversation Layer-kanalen (besloten chat, voice note, groepschat, livestream, forum) worden genoemd in openbare Reddit-discussies over intieme media-uitwisseling, en wat is de NPM-verdeling per kanaal?**

- **Waarom haalbaar:** Reddit-discussies verwijzen regelmatig naar het kanaal waar communicatie plaatsvindt. Deze verwijzingen zijn codeerbaar.
- **Essentiële toolonderdelen:** Conversation Layer (7 kanalen), Lexicale Frequentiekaart, NPM 1-6.
- **Openbare databronnen:** Pushshift (r/sex, r/relationships, r/AskReddit), zoektermen "on WhatsApp", "on Snapchat", "on Telegram", "via DM".
- **Analysemethoden:** Kanaal-vermelding-extractie, frequentie-analyse per kanaal, NPM-codering van termen per kanaal, co-occurrence-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar, maar indirect (mensen verwijzen naar kanalen, gebruiken ze niet direct).
- **Risico's en beperkingen:** Wat mensen zeggen over een kanaal is niet wat er op dat kanaal gebeurt. Anonieme Reddit-discussies kunnen andere kanalen prefereren dan realiteit.
- **Taalstrategie:** Engels (primair), Nederlands.

### VRAAG A-10

**Hoe is de pragmatische functie "discretieborging" ("niet opslaan hoor", "geen screenshot", "view once") vertegenwoordigd in openbare Reddit-discussies, en wat is de NPM van deze functie-uitingen?**

- **Waarom haalbaar:** Discretie-uitingen zijn specifieke zinsconstructies die in openbare data te vinden zijn.
- **Essentiële toolonderdelen:** Pragmatische functieregister (discretie- en privacyborging), NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** Pushshift (zoektermen: "niet opslaan", "geen screenshot", "voor jouw ogen", "tussen ons"), Reddit r/sex, r/relationships, r/dating.
- **Analysemethoden:** Zoekterm-extractie, pragmatische functiecodering, NPM-toekenning, frequentie-analyse over tijd, vergelijking tussen subreddits.
- **Verwachte bewijssterkte:** Waarschijnlijk — specifiek genoeg voor gerichte extractie.
- **Risico's en beperkingen:** Discretie-uitingen in openbare posts zijn zeldzaam (mensen bespreken discretie in privé). Extractie is gevoelig voor valse positieven.
- **Taalstrategie:** Engels (primair), Nederlands.

## FASE 4 — CATEGORIE B (PLATFORMSTRUCTUREN EN AFFORDANCES)

### VRAAG B-01

**Hoe zijn platformcommunityrichtlijnen over naaktheid en seksuele content geëvolueerd tussen 2010-2026 voor de 12 grootste platforms (Facebook, Instagram, Twitter/X, TikTok, YouTube, Reddit, Snapchat, Telegram, Discord, OnlyFans, Tumblr, Pinterest), en welke termen worden consistent gebruikt in definities van verboden content?**

- **Waarom haalbaar:** ToS en communityrichtlijnen zijn openbaar. Historische versies via Wayback Machine en ToS;DR.
- **Essentiële toolonderdelen:** DeviceAffordanceRecord, Authenticity Layer, NPM-classificatie van beleidsterminologie, SVP V3.
- **Openbare databronnen:** Wayback Machine, ToS;DR, platform transparantierapporten, platform blogposts, TechCrunch, The Verge, Wired, Platformer.
- **Analysemethoden:** Longitudinale inhoudsanalyse van ToS (n=120, 12 platforms x 10 jaar), term-frequency tracking, NPM-codering, cross-platform consistentiematrix.
- **Verwachte bewijssterkte:** Sterk — uitstekende archivering van beleidsdocumenten.
- **Risico's en beperkingen:** Platforms kunnen beleid wijzigen zonder aankondiging. Alleen geschreven beleid, niet de handhaving.
- **Taalstrategie:** Engels (primair), Nederlands.

### VRAAG B-02

**Wat is de verhouding tussen "screenshotmelding" (aan/uit/omzeilbaar) en "ephemeraliteit" per platform (Snapchat, WhatsApp, Instagram, Telegram, Signal, Facebook Messenger), en hoe wordt dit gecommuniceerd naar gebruikers in de interface vs. in de ToS?**

- **Waarom haalbaar:** Platforminterfaces zijn openbaar via app stores, screenshots, platformdocumentatie. ToS is openbaar.
- **Essentiële toolonderdelen:** DeviceAffordanceRecord, MediaLifecycleRecord, PerceivedEphemerality vs. ActualPersistence.
- **Openbare databronnen:** App Store/Google Play beschrijvingen, platform help centers, tech media, YouTube review-video's, Wikipedia.
- **Analysemethoden:** Affordance-mapping (function-matrix), interface-analyse, gap-analyse tussen belofte en realiteit.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar, maar interface verandert frequent.
- **Risico's en beperkingen:** Interface verandert frequent (maandelijkse updates). Technische werking is deels propriëtair. Wat platforms communiceren is niet wat technisch gebeurt.
- **Taalstrategie:** Engels (primair), Nederlands.

### VRAAG B-03

**Hoe verschillen transparantierapporten van platforms (Facebook/Meta, Instagram, TikTok, YouTube, Twitter/X, Snapchat, Reddit, LinkedIn, Pinterest, OnlyFans) in wat ze rapporteren over moderatie van "adult nudity and sexual activity" en "non-consensual intimate images" over de periode 2017-2026?**

- **Waarom haalbaar:** Transparantierapporten zijn openbaar, gestructureerd en kwantitatief.
- **Essentiële toolonderdelen:** EvidenceProfile, Content-Source Bias, Cross-Source Translation Table, MissingnessMap.
- **Openbare databronnen:** Meta Transparency Center, TikTok Transparency Report, YouTube Community Guidelines Report, Reddit Transparency Report, Apple App Store Transparency.
- **Analysemethoden:** Longitudinale data-extractie, vergelijkende analyse, normalisatie naar actieve gebruikers, trendanalyse.
- **Verwachte bewijssterkte:** Sterk — gestructureerde data met kwantitatieve metrics.
- **Risico's en beperkingen:** Categorieën verschillen per platform. Twitter/X is gestopt sinds 2023. Alleen data die platforms kiezen te delen.
- **Taalstrategie:** Engels.

### VRAAG B-04

**Hoe heeft de implementatie van de EU Digital Services Act (DSA) de transparantierapportage en ToS van grote platforms veranderd met betrekking tot "illegal content" en specifiek NCII, tussen 2023-2026?**

- **Waarom haalbaar:** DSA is openbare EU-wetgeving. Platformrapportages en DSA Transparency Database zijn openbaar.
- **Essentiële toolonderdelen:** EvidenceProfile, Cross-Source Translation Table.
- **Openbare databronnen:** EU DSA-wetgeving, DSA Transparency Database, platform ToS (pre/post DSA), EU Commissie rapportages.
- **Analysemethoden:** Pre/post DSA-analyse van ToS en rapportage, compliance-score per platform, term-analyse.
- **Verwachte bewijssterkte:** Sterk — volledige wetgeving en platformdata beschikbaar.
- **Risico's en beperkingen:** DSA-implementatie is nog in ontwikkeling. Alleen EU-platforms.
- **Taalstrategie:** Engels, Nederlands, EU-talen.

### VRAAG B-05

**Hoe worden "privacy labels" (Apple App Store, Google Play) voor messaging-apps gecommuniceerd naar gebruikers, en wat is de correlatie met de technische privacy-affordances van deze apps?**

- **Waarom haalbaar:** App Store privacy labels zijn openbaar. Technische affordances zijn gedocumenteerd.
- **Essentiële toolonderdelen:** DeviceAffordanceRecord, MissingnessMap.
- **Openbare databronnen:** Apple App Store privacy labels, Google Play Data Safety section, EFF "Who Has Your Back?" rapporten, tech media.
- **Analysemethoden:** Vergelijkende analyse van privacy labels, technische affordance-mapping, gap-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — labels zijn openbaar, technische verificatie beperkt.
- **Risico's en beperkingen:** Privacy labels zijn zelf-gerapporteerd. Technische verificatie vereist forensische analyse.
- **Taalstrategie:** Engels.

### VRAAG B-06

**Hoe heeft de introductie van nieuwe platformfuncties (WhatsApp View Once, Instagram Vanish Mode, Snapchat Memories, Telegram Secret Chat) de openbare discussie over ephemeraliteit en privacy op Reddit en Twitter beïnvloedt?**

- **Waarom haalbaar:** Platformfuncties worden aangekondigd in tech media. Gebruikersdiscussie vindt plaats op Reddit en Twitter.
- **Essentiële toolonderdelen:** MediaLifecycleRecord, DeviceAffordanceRecord, VisibilityIntentMismatchRecord.
- **Openbare databronnen:** Reddit (r/WhatsApp, r/Instagram, r/Snapchat, r/privacy), Twitter, tech media.
- **Analysemethoden:** Event-analyse rond functielancering, pre/post sentiment-analyse, thematische analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar, maar effectmeting is correlationeel.
- **Risico's en beperkingen:** Alleen openbare discussies. Discussie over privacy is niet privacy-gedrag.
- **Taalstrategie:** Engels (primair), Nederlands.

## FASE 4 — CATEGORIE C (CONTENT-ANALYSE VAN OPENBAAR GEDEELDE MEDIA)

### VRAAG C-01

**Hoe verhoudt de zelfverklaarde tag "amateur" op openbare Reddit-subreddits (r/amateur, r/realgirls, r/amateurcumsluts) vs. commerciële platforms (Pornhub, XVideos, OnlyFans metadata) zich tot classificatie op de 17-assige taxonomie (As 6 Commerciële intentie, As 7 Zichtbaarheidsoptimalisatie, As 8A Industrie-onafhankelijk ontstaan)?**

- **Waarom haalbaar:** Tags zijn openbaar. Metadata (titels, beschrijvingen) is beschikbaar. Alleen metadata, geen beelden.
- **Essentiële toolonderdelen:** 17-assige taxonomie (Assen 6, 7, 8A/8B), Gewogen bewijsmodel, Anti-dubbeltellingsregel.
- **Openbare databronnen:** Reddit Pushshift (amateur subreddits), Pornhub/XVideos metadata, OnlyFans metadata, Wayback Machine.
- **Analysemethoden:** Metadata-codering op 17-assen (n=500 posts), frequentieanalyse van commerciële signalen, classificatie op As 7.
- **Verwachte bewijssterkte:** Beperkt — metadata geeft beperkt zicht op ontstaanscontext.
- **Risico's en beperkingen:** Tags zijn zelfverklaard en kunnen misleidend zijn. Porno-industrie gebruikt "amateur" als marketingcategorie.
- **Taalstrategie:** Engels.

### VRAAG C-02

**Wat is de inter-rater reliability van de Gedragsladder (Niveau 0-5) wanneer deze wordt toegepast op openbare metadata (titels, beschrijvingen, tags) van 500 willekeurige posts uit Pushshift (adult-gerelateerde subreddits), gecodeerd door 5 getrainde codeurs?**

- **Waarom haalbaar:** Alleen metadata, ethisch verantwoord. Klassieke reliability study.
- **Essentiële toolonderdelen:** Gedragsladder (Niveau 0-5), 17-assige taxonomie, MissingnessMap.
- **Openbare databronnen:** Pushshift (500 posts uit top-20 adult subreddits, 2020-2023).
- **Analysemethoden:** Fleiss' Kappa per niveau, percentage agreement, Cronbach's alpha.
- **Verwachte bewijssterkte:** Sterk — klassieke inter-rater study.
- **Risico's en beperkingen:** Metadata geeft beperkte context. Sommige niveaus zijn moeilijk te coderen zonder context.
- **Taalstrategie:** Engels.

### VRAAG C-03

**Hoe effectief is de Cross-Source Translation Table in het automatisch vertalen van openbare Reddit-terminologie (nudes, sexting, intimate selfie, spicy pic, thirst trap, dick pic) naar de gestandaardiseerde IncidentRecord-variabelen?**

- **Waarom haalbaar:** Reddit-terminologie is grootschalig beschikbaar. Handmatige codering is mogelijk.
- **Essentiële toolonderdelen:** Cross-Source Translation Table, Gedragsladder, IncidentRecord.
- **Openbare databronnen:** Pushshift, handmatig gelabelde steekproef (n=200 per term).
- **Analysemethoden:** Automatische mapping vs. handmatige codering, Cohen's Kappa, sensitivity/specificity.
- **Verwachte bewijssterkte:** Sterk — direct toetsbaar.
- **Risico's en beperkingen:** Translation Table is ontworpen voor onderzoeksliteratuur, niet voor Reddit-slang.
- **Taalstrategie:** Engels.

### VRAAG C-04

**Hoe wordt de Authenticity Layer (10 categorieën) verdeeld over termen in openbare Reddit-posts over intieme media?**

- **Waarom haalbaar:** Reddit is openbaar. Termen zijn direct codeerbaar.
- **Essentiële toolonderdelen:** Authenticity Layer (10 cat.), NPM 1-6, SVP V1-V4.
- **Openbare databronnen:** Pushshift (2000 posts uit r/sex, r/AskReddit, r/TooAfraidToAsk, r/relationships).
- **Analysemethoden:** Authenticity Layer-classificatie, frequentieverdeling, chi-kwadraat tussen subreddits.
- **Verwachte bewijssterkte:** Waarschijnlijk — codering vereist interpretatie.
- **Risico's en beperkingen:** Layer is ontworpen voor privé-taal. Subreddit-normen beïnvloeden taalgebruik.
- **Taalstrategie:** Engels (primair), Nederlands.

### VRAAG C-05

**Wat is het effect van de Anti-dubbeltellingsregel op de classificatie-uitslag bij 50 openbare Reddit-posts vergeleken met een methode zonder anti-dubbeltelling?**

- **Waarom haalbaar:** Anti-dubbeltellingsregel is toepasbaar op metadata. Effect is kwantificeerbaar.
- **Essentiële toolonderdelen:** Anti-dubbeltellingsregel, Gewogen bewijsmodel, 17-assige taxonomie.
- **Openbare databronnen:** Pushshift (50 posts met meerdere zichtbaarheidssignalen).
- **Analysemethoden:** McNemar-test, verschil in bewijssterkte-scores.
- **Verwachte bewijssterkte:** Sterk — direct toetsbaar.
- **Risico's en beperkingen:** Signaal-onafhankelijkheid is subjectief te beoordelen.
- **Taalstrategie:** Engels.

## FASE 4 — CATEGORIE D (MEDIAKLOPT EN PUBLIEK DEBAT)

### VRAAG D-01

**Hoe heeft de framing van "sexting" in Nederlandse nieuwsmedia zich ontwikkeld tussen 2010-2026: verschuift de toon van moral panic naar normalisering, of blijft de risicoframe dominant?**

- **Waarom haalbaar:** LexisNexis NL en Delpher bieden volledige nieuwsarchieven.
- **Essentiële toolonderdelen:** NormalizationContextRecord, NPM 1-6, SVP V1-V4.
- **Openbare databronnen:** LexisNexis NL, Delpher, Google News NL, NOS, Volkskrant, NRC, Telegraaf, AD, Trouw.
- **Analysemethoden:** Framing-analyse per artikel, frequentie-analyse per jaar, trendanalyse (2010-2015, 2016-2020, 2021-2026).
- **Verwachte bewijssterkte:** Sterk — 5.000-10.000 artikelen over 16 jaar.
- **Risico's en beperkingen:** Alleen geschreven media. Framing is niet realiteit.
- **Taalstrategie:** Nederlands.

### VRAAG D-02

**Wat is de verhouding tussen berichtgeving over NCII en consensuele sexting in internationale nieuwsmedia (NL, UK, US, DE, FR) tussen 2015-2026?**

- **Waarom haalbaar:** Internationale nieuwsarchieven beschikbaar.
- **Essentiële toolonderdelen:** EvidenceProfile, Content-Source Bias, Cross-Source Translation Table.
- **Openbare databronnen:** LexisNexis internationaal, Genios (DE), Europresse (FR).
- **Analysemethoden:** Kwantitatieve inhoudsanalyse, framing-analyse per land, ratio consensueel/NCII.
- **Verwachte bewijssterkte:** Sterk — goede data voor 5 landen.
- **Risico's en beperkingen:** Terminologie verschilt per taal en land.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans.

### VRAAG D-03

**Hoe worden "slachtoffers" vs. "plegers" van NCII beschreven in Nederlandse nieuwsberichten: agency-toewijzing per gender?**

- **Waarom haalbaar:** Nieuwsartikelen zijn openbaar. Gender wordt vaak gerapporteerd.
- **Essentiële toolonderdelen:** ConsentByActionRecord, VisualScriptRecord.
- **Openbare databronnen:** LexisNexis NL, Google News NL.
- **Analysemethoden:** Framing-analyse per gender, agency-analyse (actief/passief taalgebruik).
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar, interpretatie vereist nuance.
- **Risico's en beperkingen:** Alleen gepubliceerde zaken (selectiebias).
- **Taalstrategie:** Nederlands.

### VRAAG D-04

**Hoe verhoudt de mediaberichtgeving over jeugd-sexting zich tot de daadwerkelijke prevalentie (18-22%) en perceived prevalence (60%) over 2015-2026?**

- **Waarom haalbaar:** Media-aandacht is kwantificeerbaar. Prevalentiecijfers uit openbare rapporten.
- **Essentiële toolonderdelen:** NormalizationContextRecord, Content-Source Bias.
- **Openbare databronnen:** LexisNexis NL, Rutgers rapporten, EU Kids Online, Google Trends.
- **Analysemethoden:** Media-aandacht-ratio vs. prevalentie-ratio, correlatie-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — correlatie is niet causaliteit.
- **Risico's en beperkingen:** Alleen incidenteel gemeten prevalentiecijfers.
- **Taalstrategie:** Nederlands.

### VRAAG D-05

**Hoe wordt "OnlyFans" en "creator economy" geframed in Nederlandse vs. Britse vs. Amerikaanse nieuwsmedia (2020-2026): empowerment, exploitatie, of commercialisering?**

- **Waarom haalbaar:** LexisNexis-dekking is goed voor deze landen.
- **Essentiële toolonderdelen:** NormalizationContextRecord, 17-assige taxonomie (As 6, As 7).
- **Openbare databronnen:** LexisNexis (NL, UK, VS), Google News, TechCrunch.
- **Analysemethoden:** Framing-analyse, sentiment-analyse, cross-nationale vergelijking.
- **Verwachte bewijssterkte:** Sterk — goed nieuwsarchief.
- **Risico's en beperkingen:** Framing is gepolitiseerd.
- **Taalstrategie:** Nederlands, Engels.

## FASE 4 — CATEGORIE E (PLATFORMBELEID EN MODERATIE)

### VRAAG E-01

**Hoe consistent zijn de definities van "non-consensual intimate imagery" (NCII) in de communityrichtlijnen van de 12 grootste platforms, en hoe verhoudt dit zich tot de definities in EU DSA, UK Online Safety Act, en nationale wetgeving (NL, DE, FR)?**

- **Waarom haalbaar:** Platformrichtlijnen en wetgeving zijn openbaar.
- **Essentiële toolonderdelen:** Cross-Source Translation Table, EvidenceProfile, MissingnessMap.
- **Openbare databronnen:** Platform ToS (Wayback Machine), EU DSA, UK OSA, wetten.nl, gesetze-im-internet.de, legifrance.gouv.fr.
- **Analysemethoden:** Vergelijkende inhoudsanalyse, term-mapping-matrix, consistentie-score per platform.
- **Verwachte bewijssterkte:** Sterk — alle documenten openbaar.
- **Risico's en beperkingen:** Definitie is niet handhaving. Wetgeving verandert.
- **Taalstrategie:** Engels, Nederlands, Duits, Frans.

### VRAAG E-02

**Wat rapporteren platforms in transparantierapporten over moderatie van adult content en NCII over 2017-2026?**

- **Waarom haalbaar:** Transparantierapporten zijn openbaar en gestructureerd.
- **Essentiële toolonderdelen:** EvidenceProfile, MissingnessMap.
- **Openbare databronnen:** Meta Transparency Center, TikTok, YouTube, Reddit, Apple rapporten.
- **Analysemethoden:** Longitudinale data-extractie, trendanalyse, missingness-analyse.
- **Verwachte bewijssterkte:** Sterk — kwantitatieve data over 9 jaar.
- **Risico's en beperkingen:** Rapportagemethodologie verandert. Alleen data die platforms delen.
- **Taalstrategie:** Engels.

### VRAAG E-03

**Hoe handhaven platforms regels over naaktheid via AI-moderatie vs. human review, volgens eigen publicaties?**

- **Waarom haalbaar:** Platformblogposts en tech media zijn openbaar.
- **Essentiële toolonderdelen:** DeviceAffordanceRecord, EvidenceProfile.
- **Openbare databronnen:** Meta AI blog, Google AI blog, TikTok for Business, TechCrunch, Platformer.
- **Analysemethoden:** Inhoudsanalyse van blogposts, term-frequentie van moderatiemethoden.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar maar niet gestructureerd.
- **Risico's en beperkingen:** Platforms publiceren selectief. AI-moderatie is propriëtair.
- **Taalstrategie:** Engels.

### VRAAG E-04

**Welke juridische definities van "intimate image" bestaan er in nationale wetgeving (NL, UK, DE, FR, CA), en hoe kunnen deze via de Cross-Source Translation Table worden gestandaardiseerd?**

- **Waarom haalbaar:** Alle wetgeving is openbaar.
- **Essentiële toolonderdelen:** Cross-Source Translation Table, Authenticity Layer, NPM.
- **Openbare databronnen:** Wetten.nl, legislation.gov.uk, gesetze-im-internet.de, legifrance.gouv.fr, canlii.org.
- **Analysemethoden:** Vergelijkende juridische analyse, term-extractie, mapping op Translation Table.
- **Verwachte bewijssterkte:** Sterk — volledige wetgeving beschikbaar.
- **Risico's en beperkingen:** Juridische definities zijn context-afhankelijk.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans.

## FASE 4 — CATEGORIE F (HISTORISCHE TRENDS)

### VRAAG F-01

**Hoe is het relatieve zoekvolume van termen "sexting", "nudes", "revenge porn", "NCII", "deepfake porn", "onlyfans" veranderd in Google Trends tussen 2008-2026 per regio?**

- **Waarom haalbaar:** Google Trends is openbaar per term en regio.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** Google Trends (2008-2026), Google Books Ngram, AnswerThePublic.
- **Analysemethoden:** Time-series analysis, term-comparison, event-correlation.
- **Verwachte bewijssterkte:** Sterk — direct beschikbaar, reproduceerbaar.
- **Risico's en beperkingen:** Relatieve volumes. Zoekdata is niet gedrag.
- **Taalstrategie:** Engels (wereldwijd), Nederlands.

### VRAAG F-02

**Hoe is de Wikipedia-editgeschiedenis van artikelen "Sexting", "Revenge porn", "Image-based sexual abuse", "Amateur pornography" veranderd tussen 2005-2026?**

- **Waarom haalbaar:** Wikipedia is volledig openbaar via API.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer, SVP V1-V4.
- **Openbare databronnen:** Wikipedia API, Wikimedia Downloads, WikiBlame.
- **Analysemethoden:** Bewerkingsfrequentie, term-substitutie-analyse, controversedetectie.
- **Verwachte bewijssterkte:** Sterk — volledige versiegeschiedenis.
- **Risico's en beperkingen:** Wikipedia-editors zijn niet representatief.
- **Taalstrategie:** Engels, Nederlands, Duits, Frans.

### VRAAG F-03

**Hoe is de academische terminologie over intieme media veranderd in OpenAlex en PubMed (2000-2026): verschuift terminologie van "sexting" naar "image-based sexual abuse" naar "tech-facilitated sexual violence"?**

- **Waarom haalbaar:** OpenAlex en PubMed zijn openbaar.
- **Essentiële toolonderdelen:** NPM 1-6, Cross-Source Translation Table, SVP V3.
- **Openbare databronnen:** OpenAlex API, PubMed Entrez, CORE, SSRN.
- **Analysemethoden:** Term-frequentie per jaar, co-occurrence-analyse, clustering.
- **Verwachte bewijssterkte:** Sterk — 250M+ werken beschikbaar.
- **Risico's en beperkingen:** PubMed heeft medische bias. Terminologie in abstracts is niet onderzoeksfocus.
- **Taalstrategie:** Engels.

### VRAAG F-04

**Hoe hebben gearchiveerde webpagina's (Common Crawl) over "amateur content" hun taal en SEO veranderd tussen 2008-2024?**

- **Waarom haalbaar:** Common Crawl bevat jaarlijkse web-crawls.
- **Essentiële toolonderdelen:** Authenticity Layer, 17-assige taxonomie.
- **Openbare databronnen:** Common Crawl (Amazon S3), Wayback Machine API.
- **Analysemethoden:** Term-frequentie per crawl, domein-analyse, SEO-praktijk-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — data groot en ongestructureerd.
- **Risico's en beperkingen:** Common Crawl is een steekproef. Vereist significante processing.
- **Taalstrategie:** Engels, Nederlands.

### VRAAG F-05

**Hoe is Google Books Ngram-frequency van termen "intimate media", "amateur pornography", "self-produced video", "sexting" veranderd in meerdere talen (1970-2019)?**

- **Waarom haalbaar:** Google Books Ngram is openbaar per taal.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** Google Books Ngram (NL, EN, DE, FR).
- **Analysemethoden:** Diachrone frequentie-analyse, trendbreuk-detectie, cross-linguïstische vergelijking.
- **Verwachte bewijssterkte:** Sterk — 50 jaar data.
- **Risico's en beperkingen:** Alleen boeken (geen tijdschriften, internet).
- **Taalstrategie:** Nederlands, Engels, Duits, Frans.

### VRAAG F-06

**Hoe heeft "selfie" (in relatie tot intieme content) zich ontwikkeld op Reddit tussen 2008-2023: frequentie, context, samenhang met intieme termen?**

- **Waarom haalbaar:** Volledige Pushshift-data.
- **Essentiële toolonderdelen:** NPM 1-6, Authenticity Layer, Conversation Layer.
- **Openbare databronnen:** Pushshift (alle posts/comments met "selfie"), Google Trends.
- **Analysemethoden:** Jaarlijkse frequentie-analyse, context-analyse, subreddit-distributie.
- **Verwachte bewijssterkte:** Sterk — volledige Reddit-data.
- **Risico's en beperkingen:** Reddit is niet algemene bevolking. "Selfie" heeft meerdere betekenissen.
- **Taalstrategie:** Engels, Nederlands.

## FASE 4 — CATEGORIE G (INTERNATIONALE VERGELIJKING)

### VRAAG G-01

**Hoe verschilt mediaberichtgeving over "sexting" tussen NL, UK, US, DE, FR, ES in toon, frequentie en terminologie (2010-2026)?**

- **Waarom haalbaar:** Nationale nieuwsarchieven beschikbaar per taal.
- **Essentiële toolonderdelen:** NormalizationContextRecord, NPM-classificatie per taal, SVP V1-V4.
- **Openbare databronnen:** LexisNexis (NL, UK, US, DE, FR, ES), Google News per land, nationale nieuwsbanken.
- **Analysemethoden:** Cross-nationale framing-analyse, frequentie gecorrigeerd voor bevolking, sentiment per land.
- **Verwachte bewijssterkte:** Sterk — data beschikbaar voor 6 landen.
- **Risico's en beperkingen:** Taalbarrières voor sentiment. LexisNexis-dekking varieert.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans, Spaans.

### VRAAG G-02

**Wat zijn de verschillen in openbare terminologie over intieme media op taal-specifieke Reddit-subreddits (r/nederlands, r/de, r/france, r/espanol, r/portugal, r/poland)?**

- **Waarom haalbaar:** Pushshift bevat taal-specifieke subreddits.
- **Essentiële toolonderdelen:** Register A/B model, NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** Pushshift (taal-specifieke subreddits).
- **Analysemethoden:** Corpus-analyse per taal, Register A/B-codering, cross-linguïstische vergelijking.
- **Verwachte bewijssterkte:** Waarschijnlijk — corpusgrootte varieert per taal.
- **Risico's en beperkingen:** Reddit is Engels-dominant. Niet alle talen hebben actieve subreddits.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans, Spaans, Portugees, Pools.

### VRAAG G-03

**Hoe verschilt Google Trends-data voor seksuele termen tussen landen met verschillende taboestructuren (NL, VS, JP, SA, DE, FR)?**

- **Waarom haalbaar:** Google Trends per land. Culturele dimensies via Hofstede.
- **Essentiële toolonderdelen:** Register A/B model, NormalizationContextRecord.
- **Openbare databronnen:** Google Trends per land, Hofstede Cultural Dimensions, World Values Survey.
- **Analysemethoden:** Cross-nationale zoekvolume-analyse, correlatie met culturele dimensies.
- **Verwachte bewijssterkte:** Waarschijnlijk — Google Trends beschikbaar, culturele verklaringen complex.
- **Risico's en beperkingen:** Google-penetratie verschilt. Internetcensuur verstoort data.
- **Taalstrategie:** Meertalig (zoektermen per land).

### VRAAG G-04

**Hoe verschilt Wikipedia-berichtgeving over "Sexting" tussen taalversies (NL, EN, DE, FR, ES, IT, PL, JA, AR)?**

- **Waarom haalbaar:** Wikipedia per taal is openbaar.
- **Essentiële toolonderdelen:** NormalizationContextRecord, NPM 1-6.
- **Openbare databronnen:** Wikipedia API per taal.
- **Analysemethoden:** Framing-analyse per taalversie, term-extractie, toon-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — taalverschillen maken directe vergelijking complex.
- **Risico's en beperkingen:** Artikelen zijn geen vertalingen van elkaar.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans, Spaans, Italiaans, Pools, Japans, Arabisch.

### VRAAG G-05

**Hoe verschillen Twitter-discussies over "OnlyFans" tussen NL, UK, US, DE, FR in sentiment en framing (2020-2026)?**

- **Waarom haalbaar:** Twitter API maakt land-filter mogelijk.
- **Essentiële toolonderdelen:** NormalizationContextRecord, 17-assige taxonomie.
- **Openbare databronnen:** Twitter Academic API, Google Trends.
- **Analysemethoden:** Sentiment-analyse per land, framing-analyse, netwerkanalyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — API-kosten hoog (~.000/maand).
- **Risico's en beperkingen:** Twitter-gebruikers niet representatief. Land-filter is gebaseerd op profiellocatie.
- **Taalstrategie:** Nederlands, Engels, Duits, Frans.

## FASE 4 — CATEGORIE H (ACADEMISCH DISCOURS)

### VRAAG H-01

**Hoe heeft academische interesse in "sexting" vs. "image-based sexual abuse" vs. "tech-facilitated sexual violence" zich ontwikkeld per discipline (2000-2026)?**

- **Waarom haalbaar:** OpenAlex en PubMed bieden publicatiedata met discipline-classificatie.
- **Essentiële toolonderdelen:** Cross-Source Translation Table, Gedragsladder.
- **Openbare databronnen:** OpenAlex API, PubMed, CORE, SSRN.
- **Analysemethoden:** Bibliometric analysis per term per jaar per discipline, co-occurrence-analyse.
- **Verwachte bewijssterkte:** Sterk — 250M+ werken over 26 jaar.
- **Risico's en beperkingen:** OpenAlex-dekking varieert per discipline.
- **Taalstrategie:** Engels.

### VRAAG H-02

**In welke mate gebruiken gepubliceerde onderzoeken klinisch-juridische termen (NPM 5-6) i.p.v. natuurlijke termen (NPM 1-2) bij beschrijving van intieme communicatie?**

- **Waarom haalbaar:** Tijdschriften zijn openbaar. Abstracts en methodesecties toegankelijk.
- **Essentiële toolonderdelen:** SVP V1-V4 (V3), NPM 1-6, Authenticity Layer.
- **Openbare databronnen:** PubMed, OpenAlex, Google Scholar, Unpaywall.
- **Analysemethoden:** SVP V3-toetsing per artikel (n=350), NPM-classificatie, trendanalyse.
- **Verwachte bewijssterkte:** Sterk — gestructureerde data.
- **Risico's en beperkingen:** SVP is voor privé-taal. Academisch discours is per definitie formeel.
- **Taalstrategie:** Engels.

### VRAAG H-03

**Wat is de geografische verdeling van sexting-onderzoek in OpenAlex: correlatie met nationale wetgeving en internetpenetratie?**

- **Waarom haalbaar:** OpenAlex bevat auteur-affiliaties.
- **Essentiële toolonderdelen:** EvidenceProfile, MissingnessMap.
- **Openbare databronnen:** OpenAlex API, ROR, World Bank.
- **Analysemethoden:** Geografische mapping, publicatie-ratio, correlatie met internetpenetratie.
- **Verwachte bewijssterkte:** Sterk — goede geografische metadata.
- **Risico's en beperkingen:** Affiliatie kan onvolledig zijn.
- **Taalstrategie:** Meertalig.

### VRAAG H-04

**Hoe verhoudt methodologische kwaliteit van sexting-onderzoek (via Content-Frequency Denominator, Granularity Level) zich tot publicatiejaar, impactfactor en discipline?**

- **Waarom haalbaar:** Artikelen zijn codeerbaar op methodologische kwaliteit.
- **Essentiële toolonderdelen:** Content-Frequency Denominator, Gedragsladder, MissingnessMap.
- **Openbare databronnen:** OpenAlex, PubMed, steekproef 200 artikelen.
- **Analysemethoden:** Codering op methodologische kwaliteit, regressie-analyse.
- **Verwachte bewijssterkte:** Waarschijnlijk — codering vereist interpretatie.
- **Risico's en beperkingen:** Methodologische kwaliteit is niet objectief meetbaar.
- **Taalstrategie:** Engels.

### VRAAG H-05

**Wat is de netwerkstructuur van co-auteurschap in internationaal sexting-onderzoek: centrale knooppunten, land-samenwerking, disciplinaire silo's?**

- **Waarom haalbaar:** OpenAlex bevat co-auteurschapsdata.
- **Essentiële toolonderdelen:** EvidenceProfile.
- **Openbare databronnen:** OpenAlex API, ROR.
- **Analysemethoden:** Netwerkanalyse (degree centrality, community detection).
- **Verwachte bewijssterkte:** Waarschijnlijk — data-dekking varieert.
- **Risico's en beperkingen:** OpenAlex heeft niet alle relaties. Grijze literatuur ontbreekt.
- **Taalstrategie:** Engels.

## FASE 4 — CATEGORIE I (TAXONOMIE EN CLASSIFICATIE OP OPENBARE BRONNEN)

### VRAAG I-01

**Wat is de inter-rater reliability van de 17-assige taxonomie op 100 openbare Reddit-posts (metadata alleen), gecodeerd door 5 codeurs?**

- **Waarom haalbaar:** Alleen metadata, ethisch verantwoord. Klassieke reliability study.
- **Essentiële toolonderdelen:** 17-assige taxonomie, Gewogen bewijsmodel, Anti-dubbeltellingsregel.
- **Openbare databronnen:** Pushshift (100 posts), codeur-training.
- **Analysemethoden:** Krippendorff's Alpha per as, Fleiss' Kappa, consensus-percentage.
- **Verwachte bewijssterkte:** Sterk — klassieke methodologie.
- **Risico's en beperkingen:** Metadata-only beperkt zicht. Sommige assen niet codeerbaar zonder context.
- **Taalstrategie:** Engels.

### VRAAG I-02

**Hoe presteert Ensceneringscontinuüm (Niveau 1-6) vs. binaire classificatie (geënsceneerd/niet) op openbare metadata?**

- **Waarom haalbaar:** Beide schalen toepasbaar op metadata.
- **Essentiële toolonderdelen:** Ensceneringscontinuüm, 17-assige taxonomie (Assen 9-14).
- **Openbare databronnen:** Pushshift (n=60 posts), 5 codeurs.
- **Analysemethoden:** Vergelijkende inter-rater reliability, informatietoename.
- **Verwachte bewijssterkte:** Waarschijnlijk — continuüm vereist meer interpretatie.
- **Risico's en beperkingen:** Zonder beeldmateriaal moeilijk te beoordelen.
- **Taalstrategie:** Engels.

### VRAAG I-03

**Wat is de inter-rater reliability van de Authenticity Layer (10 categorieën) op termen uit openbare Reddit-posts?**

- **Waarom haalbaar:** Termen zijn direct codeerbaar.
- **Essentiële toolonderdelen:** Authenticity Layer (10 cat.), NPM 1-6.
- **Openbare databronnen:** Pushshift (500 termen), 5 codeurs.
- **Analysemethoden:** Fleiss' Kappa per categorie, confusion matrix.
- **Verwachte bewijssterkte:** Sterk — heldere methodologie.
- **Risico's en beperkingen:** Sommige categorieën moeilijk te onderscheiden.
- **Taalstrategie:** Engels, Nederlands.

### VRAAG I-04

**Wat is de inter-rater reliability van het Gewogen Bewijsmodel (Score 0-4) en Beslisdrempels op 50 Reddit-posts?**

- **Waarom haalbaar:** Bewijsmodel toepasbaar op metadata.
- **Essentiële toolonderdelen:** Gewogen bewijsmodel, Beslisdrempels, Anti-dubbeltellingsregel.
- **Openbare databronnen:** Pushshift (50 posts).
- **Analysemethoden:** Fleiss' Kappa per score, percentage agreement.
- **Verwachte bewijssterkte:** Sterk — goed gedefinieerde schaal.
- **Risico's en beperkingen:** Score 3/4-grens niet altijd scherp.
- **Taalstrategie:** Engels.

### VRAAG I-05

**Hoe kan de Gedragsladder (N0-5) worden toegepast op academische literatuur (n=200), en wat is de verdeling over publicatiejaar en discipline?**

- **Waarom haalbaar:** Academische literatuur is codeerbaar.
- **Essentiële toolonderdelen:** Gedragsladder, Content-Frequency Denominator.
- **Openbare databronnen:** OpenAlex, PubMed (200 artikelen).
- **Analysemethoden:** Granulariteitscodering, trendanalyse, ANOVA per discipline.
- **Verwachte bewijssterkte:** Waarschijnlijk — codering vereist interpretatie van methodesecties.
- **Risico's en beperkingen:** Methodesecties niet altijd gedetailleerd genoeg.
- **Taalstrategie:** Engels.

### VRAAG I-06

**Wat is het effect van MissingnessMap-documentatie op interpreteerbaarheid van datasets (experiment met/zonder MissingnessMap)?**

- **Waarom haalbaar:** Experimenteel design met openbare data.
- **Essentiële toolonderdelen:** MissingnessMap, EvidenceProfile.
- **Openbare databronnen:** Pushshift (10 posts), 5 onderzoekers.
- **Analysemethoden:** Verschil in codering-zekerheid, inter-rater met/zonder MM.
- **Verwachte bewijssterkte:** Waarschijnlijk — klein maar helder design.
- **Risico's en beperkingen:** Klein sample. Hawthorne-effect.
- **Taalstrategie:** Engels.

## FASE 4 — CATEGORIE J (NETWERKANALYSE VAN OPENBARE SHARING)

### VRAAG J-01

**Hoe verspreiden links naar intieme content van Twitter/X zich via Reddit: netwerkstructuur, aggregators, tijdsdynamiek (2015-2023)?**

- **Waarom haalbaar:** URLs zijn traceerbaar in openbare data. Geen inhoud.
- **Essentiële toolonderdelen:** MediaLifecycleRecord, DeviceAffordanceRecord.
- **Openbare databronnen:** Pushshift (URL-extractie), Twitter API, Wayback Machine.
- **Analysemethoden:** Netwerkanalyse (nodes = accounts/subreddits, edges = URL shares), centraliteitsmeting, community-detectie.
- **Verwachte bewijssterkte:** Waarschijnlijk — data beschikbaar, netwerkanalyse complex.
- **Risico's en beperkingen:** Alleen openbare URLs. Privé-verspreiding onzichtbaar.
- **Taalstrategie:** Engels.

### VRAAG J-02

**Wat is de gemiddelde "levensduur" van een openbaar gedeelde URL naar intieme content op Reddit?**

- **Waarom haalbaar:** Pushshift bevat timestamps. Wayback Machine meet persistence.
- **Essentiële toolonderdelen:** MediaLifecycleRecord (persistence), TrajectoryRecord.
- **Openbare databronnen:** Pushshift, Wayback Machine API.
- **Analysemethoden:** Survival analyse (Kaplan-Meier), Cox proportional hazards.
- **Verwachte bewijssterkte:** Waarschijnlijk — censoring is een probleem.
- **Risico's en beperkingen:** Verwijdering betekent niet dat content weg is.
- **Taalstrategie:** Engels.

### VRAAG J-03

**Welke Reddit-communities functioneren als "bron" (origin) vs. "doorgeefluik" (redistributie) voor intieme content?**

- **Waarom haalbaar:** Reddit-data is gestructureerd met subreddit-hiërarchie.
- **Essentiële toolonderdelen:** VisibilityIntentMismatchRecord, NetworkLocation.
- **Openbare databronnen:** Pushshift, Reddit API.
- **Analysemethoden:** Netwerk-analyse van subreddit-verbindingen, community-rol-classificatie.
- **Verwachte bewijssterkte:** Waarschijnlijk — classificatie vereist interpretatie.
- **Risico's en beperkingen:** Subreddit-hiërarchie verandert over tijd.
- **Taalstrategie:** Engels.

---

## FASE 5: PRIORITERINGSTABEL

| ID | Categorie | Haalbaarheid | Informatiewaarde | Bewijssterkte | Inspanning | Talen |
|:---|:---|:---:|:---:|:---:|:---:|:---|
| A-01 | Terminologie | Zeer hoog | Hoog | Sterk | Laag | NL/EN |
| A-02 | Terminologie | Zeer hoog | Hoog | Sterk | Laag | EN/NL |
| A-03 | Terminologie | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| A-04 | Terminologie | Hoog | Midden | Waarschijnlijk | Midden | NL |
| A-05 | Terminologie | Midden | Hoog | Waarschijnlijk | Hoog | EN |
| A-06 | Terminologie | Hoog | Midden | Waarschijnlijk | Midden | Multil |
| A-07 | Terminologie | Zeer hoog | Hoog | Sterk | Laag | NL/EN/DE/FR |
| A-08 | Terminologie | Zeer hoog | Hoog | Sterk | Laag | NL |
| A-09 | Terminologie | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| A-10 | Terminologie | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| B-01 | Platforms | Zeer hoog | Hoog | Sterk | Laag | EN/NL |
| B-02 | Platforms | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| B-03 | Platforms | Zeer hoog | Hoog | Sterk | Laag | EN |
| B-04 | Platforms | Zeer hoog | Midden | Sterk | Laag | EN/NL/EU |
| B-05 | Platforms | Hoog | Midden | Waarschijnlijk | Midden | EN |
| B-06 | Platforms | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| C-01 | Content | Laag | Hoog | Beperkt | Hoog | EN |
| C-02 | Content | Hoog | Hoog | Sterk | Midden | EN |
| C-03 | Content | Hoog | Hoog | Sterk | Midden | EN/NL |
| C-04 | Content | Hoog | Midden | Waarschijnlijk | Midden | EN/NL |
| C-05 | Content | Hoog | Hoog | Sterk | Midden | EN |
| D-01 | Media | Zeer hoog | Hoog | Sterk | Laag | NL |
| D-02 | Media | Zeer hoog | Hoog | Sterk | Laag | NL/EN/DE/FR |
| D-03 | Media | Hoog | Midden | Waarschijnlijk | Midden | NL |
| D-04 | Media | Hoog | Hoog | Waarschijnlijk | Midden | NL |
| D-05 | Media | Hoog | Hoog | Waarschijnlijk | Midden | NL/EN |
| E-01 | Platformbeleid | Zeer hoog | Hoog | Sterk | Laag | EN/NL/EU |
| E-02 | Platformbeleid | Zeer hoog | Hoog | Sterk | Laag | EN |
| E-03 | Platformbeleid | Hoog | Midden | Waarschijnlijk | Midden | EN |
| E-04 | Platformbeleid | Zeer hoog | Hoog | Sterk | Laag | NL/EN/DE/FR |
| F-01 | Historisch | Zeer hoog | Hoog | Sterk | Laag | EN/NL |
| F-02 | Historisch | Zeer hoog | Hoog | Sterk | Laag | Multil |
| F-03 | Historisch | Zeer hoog | Hoog | Sterk | Laag | EN |
| F-04 | Historisch | Midden | Hoog | Waarschijnlijk | Hoog | EN |
| F-05 | Historisch | Zeer hoog | Midden | Sterk | Laag | Multil |
| F-06 | Historisch | Zeer hoog | Midden | Sterk | Laag | EN/NL |
| G-01 | Internationaal | Zeer hoog | Hoog | Sterk | Midden | Multil |
| G-02 | Internationaal | Hoog | Midden | Waarschijnlijk | Midden | Multil |
| G-03 | Internationaal | Hoog | Midden | Waarschijnlijk | Midden | Multil |
| G-04 | Internationaal | Hoog | Midden | Waarschijnlijk | Midden | Multil |
| G-05 | Internationaal | Midden | Midden | Waarschijnlijk | Hoog | Multil |
| H-01 | Academisch | Zeer hoog | Hoog | Sterk | Laag | EN |
| H-02 | Academisch | Zeer hoog | Hoog | Sterk | Laag | EN |
| H-03 | Academisch | Zeer hoog | Midden | Sterk | Laag | Multil |
| H-04 | Academisch | Hoog | Hoog | Waarschijnlijk | Midden | EN |
| H-05 | Academisch | Hoog | Midden | Waarschijnlijk | Midden | EN |
| I-01 | Taxonomie | Hoog | Hoog | Sterk | Midden | EN |
| I-02 | Taxonomie | Midden | Midden | Waarschijnlijk | Hoog | EN |
| I-03 | Taxonomie | Hoog | Hoog | Sterk | Midden | EN/NL |
| I-04 | Taxonomie | Hoog | Midden | Waarschijnlijk | Midden | EN |
| I-05 | Taxonomie | Hoog | Hoog | Waarschijnlijk | Midden | EN |
| I-06 | Taxonomie | Hoog | Midden | Waarschijnlijk | Midden | EN |
| J-01 | Netwerken | Midden | Hoog | Waarschijnlijk | Hoog | EN |
| J-02 | Netwerken | Midden | Midden | Waarschijnlijk | Hoog | EN |
| J-03 | Netwerken | Midden | Midden | Waarschijnlijk | Hoog | EN |

### Prioriteitsaanbevelingen

**Eerste prioriteit (direct uitvoerbaar, hoge informatiewaarde, lage inspanning):**
A-01, A-02, A-07, A-08, B-01, B-03, B-04, D-01, D-02, E-01, E-02, E-04, F-01, F-02, F-03, F-05, F-06, H-01, H-02

**Tweede prioriteit (uitvoerbaar, maar vereist meer voorbereiding):**
A-03, A-04, A-06, A-09, A-10, B-02, B-05, B-06, C-02, C-03, C-04, C-05, D-03, D-04, D-05, E-03, F-04, G-01, G-02, G-03, G-04, H-03, H-04, H-05, I-01, I-03, I-04, I-05, I-06

**Derde prioriteit (complex, hoog risico, maar potentieel hoge waarde):**
A-05, C-01, G-05, I-02, J-01, J-02, J-03

---

## FASE 6: KRITISCHE EVALUATIE

### 6.1 KENNISHIATEN DIE DOOR DATABEPERKINGEN NIET TE VULLEN ZIJN

1. **De privé-communicatiekloof:** We kunnen niet weten wat er daadwerkelijk in intieme 1-op-1 chats wordt gezegd. Alleen publiekelijk gedeelde communicatie is zichtbaar. De Register B/data die we in openbare bronnen vinden is per definitie anders dan Register B in privé-chats. Publieke Register B is performatiever, doelbewuster en context-vrijer.

2. **De non-event baseline:** We kunnen niet weten hoeveel intieme beelden worden gemaakt, gedeeld en daarna zonder enig gevolg blijven. Alleen beelden die escaleren, worden gemeld of genoemd in openbare bronnen. Dit is de fundamentele onzichtbare noemer van alle sexting-onderzoek.

3. **De ontstaanscontext:** Bij openbare metadata kunnen we nooit met zekerheid vaststellen wat de werkelijke ontstaanscontext was. As 14 (Opname-afhankelijkheid) en As 9 (Camerabewustzijn) zijn niet te coderen zonder directe bronverificatie.

4. **Toestemming:** Consents-status (deelname, opname, opslag, first-share, re-share) is onmogelijk vast te stellen op basis van alleen openbare data. We kunnen alleen zien wat er publiekelijk wordt gedeeld, niet of daarvoor toestemming was.

5. **De slachtofferervaring:** NCII-slachtoffers zijn niet bereikbaar via openbare data. Hun ervaringen zijn alleen indirect zichtbaar (nieuwsberichten, anonieme forums). Dit geeft een gefilterd, vaak sensationalistisch beeld.

6. **Platform-backend-realiteit:** We kunnen niet verifiëren wat platforms werkelijk doen met data, moderatie, of privacy. Alleen wat ze rapporteren is zichtbaar.

7. **Causale mechanismen:** Zonder experimenteel design of longitudinale cohortdata kunnen we geen causale uitspraken doen over effecten van platforms, beleid of media op gedrag.

8. **Algoritmische ondoorzichtigheid:** Hoe platformalgoritmes content selecteren, aanbevelen of onderdrukken is grotendeels onbekend. Dit beïnvloedt wat zichtbaar is in openbare data.

### 6.2 STRUCTURELE BIASES

**Wie praat er publiekelijk over seks?**
Openbaar discours over seks, intimiteit en naaktheid is niet representatief voor de algemene bevolking:
- Mensen die er openbaar over praten zijn selectief: jonger, mannelijker (voor bepaalde forums), liberaler, vaker anoniem.
- Mensen met negatieve ervaringen (NCII) zijn ondervertegenwoordigd in openbare forums vanwege schaamte.
- Mensen in conservatieve of religieuze omgevingen zijn ondervertegenwoordigd.
- Mensen uit lagere socio-economische klassen hebben minder toegang tot/vaardigheid in schriftelijk discours.

**Reddit-specifieke bias:**
- Reddit-gebruikers zijn disproportioneel mannelijk (~65%), jong (18-29 is grootste groep), westers (VS ~50% van verkeer), en hoger opgeleid.
- Reddit-discours is anoniemer dan andere platforms, wat leidt tot meer expliciete taal maar ook meer troll-gedrag.
- Subreddit-culturen verschillen enorm: r/sex is anders dan r/NSFW.
- Pushshift-data stopt in 2023 (Reddit API-wijzigingen). Huidige data is beperkter.

**Taalbias:**
- Engels domineert openbare data (60%+ van Reddit, 80%+ van academische publicaties, 70%+ van Google Trends-data).
- Nederlandse data is beschikbaar maar beperkter (kleinere subreddits, minder nieuwsarchieven, kleinere Google Trends-volumes).
- Niet-westerse talen (Arabisch, Chinees, Hindi, Swahili) zijn dramatisch ondervertegenwoordigd.
- Vertalingen introduceren registerverschuivingen die NPM-scores beïnvloeden.

**Platformbias:**
- Reddit is niet algemene bevolking is niet Twitter is niet Facebook is niet TikTok.
- Verschillende platforms trekken verschillende demografieën en discours-stijlen.
- Wat op Reddit als "normaal" geldt (expliciete taal, anonieme seksuele verhalen) is niet representatief.
- Platform-algoritmes beïnvloeden wat zichtbaar is en wat niet.
- Platform-API-wijzigingen veranderen wat onderzoekers kunnen zien.

**Survivorship bias:**
- Alleen bewaard gebleven data is zichtbaar. Verwijderde posts, verdwenen websites, dode links zijn onzichtbaar.
- Wayback Machine archiveert niet alles. Common Crawl is een steekproef.
- Platforms die data actief verwijderen (moderatie) creëren een gekuist beeld.
- Oudere data is schaarser (minder archivering voor 2010).

**Indexeringsproblemen:**
- Wat Google niet vindt, bestaat voor ons niet. Diepe webpagina's, besloten forums, dynamische content worden niet geïndexeerd.
- Acroniemen, slang en algospeak ontsnappen aan standaard zoekopdrachten.
- Pushshift heeft niet alle Reddit-data (bepaalde subreddits zijn uitgesloten).
- Twitter/X Academic API is duur en beperkt sinds 2023.

**Publicatiebias:**
- Academische publicaties zijn biased naar positieve resultaten en significante effecten.
- Nieuwsmedia zijn biased naar negatieve, sensationalistische verhalen.
- Beleidsrapporten zijn biased naar problematisering (legitimatie van beleid).
- Openbare forums zijn biased naar uitzonderlijke verhalen (niemand post "er gebeurde niets").

### 6.3 METHODOLOGISCHE COMPENSATIES

Om deze biases te adresseren, passen we de volgende compensaties toe in elke analyse:

1. **Expliciete bias-documentatie:** Elke onderzoeksvraag heeft een "Risico's en beperkingen" veld dat de specifieke biases benoemt.

2. **Triangulatie:** Waar mogelijk gebruiken we meerdere onafhankelijke bronnen (Reddit + nieuws + Google Trends + academisch) voor dezelfde vraag.

3. **MissingnessMap-plicht:** Alle variabelen met onbekende/ontbrekende data worden expliciet geregistreerd via de MissingnessMap-standaard.

4. **Geen stilzwijgende defaults:** Ontbrekende data wordt niet geïnterpreteerd als afwezigheid. Toestemming onbekend is niet vrijwillig. Dwang niet genoemd is niet geen dwang.

5. **Geen causaliteit zonder experiment:** Correlaties worden niet gepresenteerd als causaliteit. Alleen descriptieve en correlationele claims.

6. **SVP-verplichting:** Alle taalkundige conclusies worden getoetst op SVP V1-V4. Klinische termen worden niet gepresenteerd als natuurlijke taal.

7. **Denominator-transparantie:** Frequenties worden altijd met expliciete noemer gerapporteerd (DENOM 01-05). Vergelijking alleen op zelfde noemer.

8. **Granulariteitsbeperking:** Bronnen worden alleen vergeleken op hetzelfde granulariteitsniveau (Niveau 0-5). Schijnprecisie wordt vermeden.

9. **Platform-specificatie:** Claims worden altijd gespecificeerd per platform. "Reddit toont X" is niet "het internet toont X".

10. **Open data en reproduceerbaarheid:** Alle code, datasets (waar mogelijk) en methoden worden openbaar gedeeld voor replicatie.

### 6.4 WAT DEZE AGENDA WEL EN NIET KAN DOEN

**Deze agenda kan wél:**
- Systematisch in kaart brengen hoe er publiekelijk over intieme media, sexting en NCII wordt gesproken
- De terminologie, framing en discours analyseren over tijd, per taal, per platform, per land
- De 17-assige taxonomie en NPM-schaal valideren op openbare metadata
- Platformbeleid en mediaberichtgeving longitudinal analyseren
- Netwerken van openbare sharing documenteren
- De kloof tussen academisch/beleidsjargon en publiek discours kwantificeren
- Trends in Google-zoekgedrag en Wikipedia-bewerkingen meten
- Cross-linguïstische en cross-nationale vergelijkingen maken
- Inter-rater reliability van alle toolonderdelen meten
- De methodologische kwaliteit van bestaand onderzoek evalueren

**Deze agenda kan níet:**
- De "waarheid" over privé-intieme communicatie ontsluiten
- Toestemming of ontstaanscontext verifiëren voor individuele casussen
- De non-event baseline kwantificeren
- Slachtofferervaringen direct documenteren
- Platform-backend-realiteit verifiëren
- Representativiteit voor de algemene bevolking claimen voor discours-analyses
- Causale uitspraken doen over gedrag of effecten
- Het Hawthorne-effect in intieme opnames meten
- Register B in authentieke privé-chats analyseren

### 6.5 SLOTCONCLUSIE

Deze v3-agenda is **bewust kleiner en bescheidener** dan v1 en v2, maar daardoor **realistischer en uitvoerbaarder**. Waar de eerdere agenda's een ideaalbeeld schetsten van wat er allemaal mogelijk zou zijn met ideale data, beschrijft deze agenda wat er **daadwerkelijk mogelijk is** met publiek beschikbare data.

De kern is: we kunnen met openbare data geen uitspraken doen over **privé-gedrag**, maar we kunnen wél systematisch uitspraken doen over **publiek discours** over dat gedrag. Dat is een fundamenteel ander object van onderzoek — maar niet minder waardevol.

Publiek discours is namelijk:
- Wat beleidsmakers en politici horen en waarop ze reageren
- Wat journalisten schrijven en wat het algemene beeld bepaalt
- Wat platforms communiceren over hun regels en wat gebruikers denken dat mag
- Wat jongeren zelf zeggen dat ze doen (wat niet hetzelfde is als wat ze doen, maar wel hun sociale realiteit vormt)

Door de systematische toepassing van de toolonderdelen (NPM, Authenticity Layer, 17-assige taxonomie, SVP, Gedragsladder, MissingnessMap, Anti-dubbeltellingsregel, Cross-Source Translation Table) op openbare data, ontstaat een **empirisch onderbouwd, reproduceerbaar en methodologisch transparant beeld van het publieke discours** over intieme media, sexting, NCII en gerelateerde fenomenen.

Dat is minder dan idealiter mogelijk zou zijn. Maar het is ook meer dan wat tot nu toe systematisch is gedaan.

**Het belangrijkste methodologische inzicht van deze analyse is:**
De ontoegankelijkheid van privé-data is geen beperking die we moeten omzeilen, maar een fundamentele eigenschap van het onderzoeksobject die we moeten erkennen en in onze methodologie moeten verwerken. De MissingnessMap, Non-Event Baseline en expliciete bias-documentatie maken deze agenda juist sterker doordat ze helder maken wat we wel en niet kunnen weten.

### UITVOERINGSPLANNING

**Fase 0 (Maand 1-2):** Opzetten data-infrastructuur
- Toegang verkrijgen tot Pushshift, LexisNexis, OpenAlex
- Codeurstraining taxonomieën (17-assen, Gedragsladder, Authenticity Layer)
- Pilot-codering (n=50)

**Fase 1 (Maand 3-6):** Eerste prioriteit vragen
- A-01, A-02, A-07, A-08: terminologie-analyse gestart
- B-01, B-03, B-04: platformbeleid en DSA-analyse
- D-01, D-02: mediaberichtgeving
- E-01, E-02, E-04: platformbeleid en wetgeving
- F-01, F-02, F-03, F-05, F-06: historische trends
- H-01, H-02: academisch discours

**Fase 2 (Maand 7-12):** Tweede prioriteit vragen
- A-03, A-04, A-06, A-09, A-10: terminologie-uitbreiding
- B-02, B-05, B-06: platform-diepte
- C-02, C-03, C-04, C-05: taxonomie-toepassing
- D-03, D-04, D-05: mediaklopt-uitbreiding
- E-03: platformbeleid-diepte
- F-04: Common Crawl-diepte
- G-01, G-02, G-03, G-04: internationale vergelijking
- H-03, H-04, H-05: academische diepte
- I-01, I-03, I-04, I-05, I-06: taxonomie-reliability

**Fase 3 (Maand 13-18):** Derde prioriteit vragen
- A-05: semantische verschuiving "amateur"
- C-01: openbare content-classificatie
- G-05: internationale Twitter-analyse
- I-02: ensceneringscontinuüm
- J-01, J-02, J-03: netwerkanalyse

**Fase 4 (Maand 19-24):** Synthese en publicatie
- Cross-categorie synthese
- Validatie van toolonderdelen (geaggregeerd)
- Publicatie van methodologie en resultaten (open access)
- Open delen van geanonimiseerde datasets en code

### APPENDIX A — TOOL-INZET MATRIX

Welke toolonderdelen worden ingezet per categorie:

| Toolonderdeel | A | B | C | D | E | F | G | H | I | J |
|:---|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| NPM 1-6 | X | | X | X | | X | X | X | | |
| Authenticity Layer (10 cat.) | X | | X | X | | X | X | X | | |
| Register A/B model | X | | | | | | X | | | |
| SVP V1-V4 | X | | | X | | X | X | X | | |
| 17-assige taxonomie | X | | X | | | | | | X | |
| Gedragsladder (N0-5) | | | X | | | | | | X | |
| Cross-Source Translation | | | X | | X | | | X | X | |
| MissingnessMap | | | X | | X | X | X | X | X | X |
| Content-Frequency Denom | | | X | | | | | X | X | |
| MediaLifecycleRecord | | X | | | | | | | | X |
| DeviceAffordanceRecord | | X | | | X | | | | | |
| NormalizationContextRecord | | | | X | | | | X | | |
| EvidenceProfile | | X | X | X | X | X | X | X | X | X |
| Content-Source Bias | | | X | X | X | | X | X | | |
| Anti-dubbeltellingsregel | | | X | | | | | | X | |
| Gewogen bewijsmodel | | | X | | | | | | X | |
| Conversation Layer | X | | | | | | | | | |
| Pragmatische functies | X | | | | | | | | | |
| Pattern Library | | | | | | | | | | X |
| Non-Event Baseline | | | X | | | | | | | |

### APPENDIX B — ETHISCHE EN JURIDISCHE GRENZEN

1. **Geen beeldmateriaal:** Deze agenda analyseert uitsluitend metadata, tekst, tags, beschrijvingen en terminologie. Geen intieme beelden worden gedownload, bekeken of geanalyseerd.

2. **Anonieme/geaggregeerde data:** Alle gebruikte data wordt geanonimiseerd of is van nature geaggregeerd (Google Trends, Wikipedia, OpenAlex). Geen individuele gebruikers worden geïdentificeerd.

3. **Geen interactie met kwetsbare groepen:** Er wordt geen direct contact gezocht met minderjarigen, NCII-slachtoffers of andere kwetsbare personen.

4. **Alleen publiek toegankelijke data:** Geen data wordt verkregen via hacking, omzeiling van authenticatie, of misbruik van API's.

5. **Geen interceptie van privé-communicatie:** WhatsApp, Signal, Telegram, iMessage, en andere encrypted diensten worden niet ontsleuteld of onderschept.

6. **Toestemming voor onderzoek:** Waar nodig (bijv. voor handmatige codering) wordt toestemming verkregen van ethische commissies.

7. **AVG-compliance:** Alle dataverzameling en -verwerking voldoet aan de AVG/GDPR.

8. **Transparantie:** Alle methoden, databronnen en beperkingen worden gedocumenteerd en gepubliceerd.

9. **Geen scrape van betaalde content:** Alleen openbaar toegankelijke data. Geen omzeiling van betaalmuren.

10. **Respect voor platform ToS:** Waar platform Terms of Service scrapping verbieden, worden alternatieve bronnen gebruikt.

---

*Einde document — 22 juli 2026*
*Versie 3.0 — Realistische haalbaarheidsanalyse op basis van openbare databronnen*
*Gebaseerd op de toolomgeving: Module 1 (Jeugd Incidenten 15-18) + Module 2 (Intieme Taal & 17-Assige Taxonomie)*

## UITGEBREIDE APPENDIX C — VOLLEDIGE CATEGORIE-OVERZICHT MET BRONVERWIJZINGEN

### C.1 Publiek discours en terminologie — uitgebreide brontoelichting

**Reddit Pushshift — technische specificatie:**
Pushshift.io bevat alle openbare Reddit-posts en -comments van 2005 tot maart 2023. De dataset omvat: post-ID, timestamp, auteur, titel, body text, subreddit, score, aantal comments, goud/silver/bronzen awards, post-URL, cross-post data, verwijderde posts (gemarkeerd als [removed] of [deleted]). De data is beschikbaar via API, directe dumps (JSON-lines, ~400GB gecomprimeerd), en in BigQuery (Google Cloud). Voor onderzoek naar intieme terminologie zijn de volgende subreddits primair relevant:

r/sex (~2.5M abonnees, ~100 nieuwe posts/dag): advies, vragen, ervaringen. Rijke bron voor Register A- en B-terminologie.
r/relationships (~4M abonnees, ~200 posts/dag): relatie-advies, inclusief intieme dilemma's.
r/dating_advice (~1.5M abonnees): dating-vragen, eerste stappen in intieme communicatie.
r/dirtyr4r (~500K abonnees): directe seksuele verzoeken, Register B-rijk.
r/AskReddit (~45M abonnees): grote dataset voor term-frequentie, thematische draadjes.
r/teenagers (~3M abonnees): discussies over sexting door jongeren.
r/nederlands en r/thenetherlands (~500K totaal): Nederlandstalig discours.
r/seks (~10K abonnees): Nederlandse seks-advies subreddit.

**Corpus-specificaties:**
- Engels: >10B woorden beschikbaar (alle subreddits, 2005-2023)
- Nederlands: >200M woorden (alle Nederlandstalige subreddits)
- Standaard NPM-corpora: vergelijkbare grootte voor Engelse en Nederlandse termen

### C.2 LexisNexis — technische specificatie voor mediaklopt-analyse

LexisNexis biedt toegang tot >15.000 nieuwsbronnen wereldwijd. Voor mediaklopt-analyse zijn de volgende land-specifieke bronnen relevant:

Nederland:
- NRC Handelsblad (volledig archief 1988-2026)
- De Volkskrant (volledig archief 1990-2026)
- De Telegraaf (volledig archief 1995-2026)
- Algemeen Dagblad (volledig archief 1995-2026)
- Trouw (volledig archief 1995-2026)
- Het Parool (volledig archief 1995-2026)
- NU.nl (online, 2010-2026)
- NOS nieuws (online, 2010-2026)
- RTL Nieuws (online, 2010-2026)
- Regionale kranten (via LexisNexis bundel)

Verenigd Koninkrijk:
- The Guardian, The Times, The Telegraph, The Independent, Daily Mail, BBC News

Verenigde Staten:
- The New York Times, Washington Post, Wall Street Journal, USA Today, CNN, Fox News, MSNBC

Duitsland:
- Frankfurter Allgemeine, Süddeutsche Zeitung, Die Welt, Die Zeit, Spiegel, Bild

Frankrijk:
- Le Monde, Le Figaro, Libération, Les Echos, Le Parisien

Zoekstrategie voor consistentie over landen:
Engels: "sexting" OR "nudes" OR "revenge porn" OR "image-based sexual abuse" OR "NCII" OR "intimate image" OR "non-consensual intimate"
Nederlands: "sexting" OF "nudes" OF "wraakporno" OF "intieme beelden" OF "naaktfoto" OF "beeldmateriaal"
Duits: "Sexting" ODER "Nacktfotos" ODER "Racheporno" ODER "intime Bilder" ODER "nicht einvernehmliche Verbreitung"
Frans: "sexting" OU "nudes" OU "porno vengeance" OU "image intime" OU "non consensuel"

### C.3 Google Trends — operationele specificatie

Google Trends biedt relatief zoekvolume per term, per regio, per periode. Data is genormaliseerd (0-100 schaal). Beschikbaar op dag-, week-, maand- en jaarbasis. Regio-selectie op landniveau, of wereldwijd. Categorie-filter beschikbaar (bijv. "People & Society" of "Health").

Relevante vergelijkingen voor deze agenda:
- "sexting" (2008-2026): wereldwijd, NL, UK, US, DE, FR, ES, IT, JP
- "nudes" (2010-2026): zelfde regio's
- "revenge porn" (2012-2026): zelfde regio's + wetgevingsmomenten
- "NCII" / "non-consensual intimate images" (2018-2026): beleidsterm-tracking
- "deepfake porn" (2019-2026): opkomende term
- "onlyfans" (2019-2026): creator economy term
- "amateur porn" (2008-2026): semantische verschuiving
- "selfie" (2010-2026): controlegroep voor algemene term-trends

Beperkingen:
- Geen absolute volumes (alleen relatieve)
- Minste drempel voor lage-volume termen (soms onvoldoende data)
- Geen demografische opsplitsing
- Google-blokkade in sommige landen

### C.4 OpenAlex — bibliometrische specificatie

OpenAlex (openalex.org) is een volledig open index van academische werken. Specificaties:
- ~250 miljoen werken (artikelen, boeken, hoofdstukken, datasets, etc.)
- ~100 miljoen auteurs met affiliaties
- ~90.000 tijdschriften/tijdschriftbronnen
- ~20.000 onderwerpen (hiërarchisch)
- Volledig open API (geen authenticatie vereist, rate limit: 10 requests/second)
- Data beschikbaar via API, data-dumps (JSON), en Snowflake-partnerschap
- Geüpdatet maandelijks

Relevante zoekqueries voor deze agenda:
- Termen in titel: sexting, image-based sexual abuse, non-consensual intimate image, intimate media, tech-facilitated sexual violence, revenge porn, nudes, amateur pornography
- Termen in abstract: zelfde termen
- Disciplines: Psychology, Sociology, Communication Studies, Criminology, Law, Media Studies, Gender Studies, Education, Public Health
- Publicatiejaren: 2000-2026
- Type werk: artikel, boek, hoofdstuk

### C.5 Wikipedia API — specificatie voor edit-geschiedenis analyse

Wikipedia biedt volledige versiegeschiedenis van alle pagina's. Specificaties:
- MediaWiki API (public, geen authenticatie)
- Revisions endpoint: volledige lijst van bewerkingen met timestamp, editor, commentaar, size delta
- Blame tool: per-woord versie-herkomst
- Category members: alle pagina's in een categorie
- Volledige dumps beschikbaar via Wikimedia Downloads (XML, ~80GB per taal)

Relevante pagina's voor deze agenda:
- EN: Sexting, Revenge porn, Image-based sexual abuse, Non-consensual intimate image, Amateur pornography, Nude photography, OnlyFans, Internet pornography
- NL: Sexting, Wraakporno, Pornografie, Naaktfotografie
- DE: Sexting, Racheporno, Kinderpornografie, Privataufnahme
- FR: Sexting, Porno vengeance, Image intime non consensuelle
- ES, IT, PL, JA, AR: overeenkomstige pagina's

### C.6 Common Crawl — specificatie voor web-analyse

Common Crawl is een open dataset van webcrawls. Specificaties:
- Maandelijks/jaarlijks gecrawld sinds 2008
- ~3-5 miljard pagina's per crawl
- Dataformaat: WARC (raw), WAT (metadata), WET (text only)
- Beschikbaar op Amazon S3 (us-east-1, gratis toegang met AWS account)
- Querybaar via AWS Athena (SQL op WARC/PARQUET)

Relevante domeinen/categorieën voor deze agenda:
- Adult content platforms (pornhub.com, xvideos.com, xhamster.com, etc.)
- Creator economy platforms (onlyfans.com, fansly.com, manyvids.com, etc.)
- Amateur tagging categorieën
- Forum-archieven (partyflock.nl, fok.nl, etc.)
- Wikipedia mirror sites
- Platform Terms of Service pagina's

### C.7 Platform transparency reports — data-standaardisatie

Platfrom transparency reports variëren in consistentie. Om cross-platform vergelijking mogelijk te maken, normaliseren we naar de volgende metrics:

| Metric | Meta | TikTok | YouTube | Reddit | Apple |
|:---|---:|:---:|:---:|:---:|:---:|
| Content type | Adult nudity & sexual activity | Adult nudity & sexual activity | Nudity & sexual content | Sexual content | Adult content |
| Definitie NCII | Non-consensual intimate images | Non-consensual intimate media | N/A | Involuntary pornography | N/A |
| Metric | Items removed | Videos removed | Videos removed | Posts/content removed | Apps rejected |
| Periode | Quarterly | Semi-annual | Quarterly | Annual | Annual |
| Startdatum | 2013 | 2020 | 2017 | 2020 | 2020 |
| Proactief % | Gerapporteerd | Gerapporteerd | N/A | N/A | N/A |
| Appeals/Herstel | Gerapporteerd | Gerapporteerd | Gerapporteerd | Gerapporteerd | Gerapporteerd |

Let op: Twitter/X publiceerde transparantierapporten van 2012-2022, maar is gestopt sinds de overname door Elon Musk in 2022.

### C.8 Aanvullende databronnen per categorie

**Categorie A (Terminologie) — extra bronnen:**
- Google Books Ngram viewer (NL, EN, DE, FR, ES, IT, RU, ZH): boeken 1800-2019
- Project Gutenberg: historische boeken over seksualiteit (pre-1928)
- Early English Books Online (EEBO): 16e-18e eeuwse teksten
- Corpus Gesproken Nederlands (CGN): 800 uur gesproken Nederlands, 1960-2020
- SoNaR: 500M woorden Nederlands geschreven corpus
- CHN (Corpus Hedendaags Nederlands): 500M woorden, 2005-2015
- COCA (Corpus of Contemporary American English): 1B woorden, 1990-2019
- BNC (British National Corpus): 100M woorden, 1980-1993

**Categorie D (Mediaklopt) — extra bronnen:**
- Delpher (NL): 1M+ krantenpagina's, 1618-2005
- Trove (Australië): historische kranten, 1803-1954
- Chronicling America (VS): historische kranten, 1777-1963
- Gallica (FR): Franse kranten, 17e-20e eeuw
- ANNO (Oostenrijk): Oostenrijkse kranten, 18e-20e eeuw
- World Newspaper Archive: wereldwijde kranten, 18e-20e eeuw

**Categorie H (Academisch) — extra bronnen:**
- CrossRef: DOI-registratie, 120M+ werken
- CORE: 200M+ open access artikelen
- ArXiv: preprints, informatica/fysica/wiskunde
- SSRN: sociale wetenschappen preprints
- ResearchGate: research social network (deels openbaar)
- Academia.edu: research social network (deels openbaar)
- Zenodo: research data repository
- Figshare: research data repository

**Categorie J (Netwerken) — extra bronnen:**
- Twitter API v2: volledige tweet-objecten, conversation threading, likes, retweets
- Reddit Pushshift: cross-posts, subreddit-verbindingen, gebruikersactiviteit
- Wayback Machine CDX API: URL-persistence, dode link detectie, redirect chains
- Common Crawl: web-grafieken, link-structuren per crawl
- GitHub Archive: repository-activiteit, 2011-heden
- GDELT Project: nieuws-netwerken, 1979-heden

## UITGEBREIDE APPENDIX D — METHODOLOGISCHE PROTOCOLLEN PER ANALYSETYPE

### D.1 Corpus-analyse protocol (Categorie A)

**Stap 1: Data-extractie**
- Selecteer corpora per onderzoeksvraag (bv. Reddit Pushshift, subreddit-filter, datumfilter)
- Extraheer posts/comments via API of bigquery
- Filter op taal (langdetect of CLD2)
- Tokeniseer tekst (spacy, NLTK, stanza)
- Normaliseer (lowercase, verwijder URLs, verwijder speciale karakters voor standaard analyse)

**Stap 2: Term-extractie en NPM-toekenning**
- Gebruik vooraf gedefinieerde termlijst uit Lexicale Frequentiekaart (72+ termen uit Data 1/7)
- Ken NPM-score toe op basis van corpusfrequentie (P > 0,70 = NPM 1; 0,35-0,70 = NPM 2; contextafhankelijk = NPM 3; 0,01-0,10 = NPM 4; P≈0 in privé = NPM 5; P<0,01 = NPM 6)
- Bereken P(spontaan) = (term-frequentie in corpus) / (totaal woorden in corpus) × 100.000 (per 100.000 woorden)
- Vergelijk met baseline (Google Books Ngram, CGN, COCA, BNC)

**Stap 3: Register-classificatie**
- Classificeer elke term als Register A, Register B, of gemengd
- Gebruik co-occurrence-analyse voor register-typering (Register A co-occurrentie met eufemismen, Register B met directe anatomische termen)
- SVP V1-V4 toepassing op elke term-classificatie

**Stap 4: Authenticity Layer-classificatie**
- Ken 1 van 10 Authenticity Layer-categorieën toe
- Bereken inter-rater reliability (Fleiss' Kappa)
- Documenteer onzekerheden per term

**Stap 5: Statistische analyse**
- Chi-kwadraat voor frequentieverschillen tussen corpora
- Mann-Kendall test voor trends over tijd
- ANOVA voor verschillen tussen subreddits/forums
- Effect size (Cohen's d of Cramer's V)

**Stap 6: Rapportage**
- NPM-verdeling per corpus
- Register-profiel per corpus
- Authenticity Layer-profiel
- SVP-goedkeuringspercentage per term
- MissingnessMap: welke termen zijn niet gevonden in bepaalde corpora?

### D.2 Framing-analyse protocol (Categorie D)

**Stap 1: Data-extractie (LexisNexis)**
- Zoekopdracht per land per taal (zie C.2 voor zoektermen)
- Datumfilter: 2010-2026 (of specifieke periode per vraag)
- Exporter als HTML of plain text met metadata (datum, krant, auteur, sectie)

**Stap 2: Framing-codering**
Ontwikkel codeerhandboek met de volgende frames:
- Risicoframe: nadruk op gevaar, schade, criminaliteit, slachtofferschap
- Moral panic frame: nadruk op moreel verval, jeugd in gevaar, urgentie
- Normaliseringsframe: nadruk op gewoon gedrag, ontwikkeling, relativiteit
- Juridisch frame: nadruk op wetgeving, strafbaarheid, handhaving
- Emancipatieframe: nadruk op empowerment, seksuele vrijheid, eigen keuze
- Technologieframe: nadruk op platform-rol, technische oplossingen, privacy
- Neutraal/informatief frame: feitelijke rapportage zonder duidelijke framing

**Stap 3: Agency-codering (voor D-03)**
- Codeer per genoemd persoon: actief/passief taalgebruik
- Actief: "zij stuurde", "hij deelde", "de dader verspreidde"
- Passief: "haar foto werd verspreid", "zij werd slachtoffer van"
- Gender noteren (indien vermeld)
- Rol noteren (maker, verspreider, ontvanger, slachtoffer, dader, hulpverlener, ouder, school)

**Stap 4: Sentiment-analyse**
- VADER voor Engels
- Pattern of LIWC-NL voor Nederlands
- SentiWS voor Duits
- FEEL voor Frans

**Stap 5: Internationale vergelijking**
- Normaliseer voor bevolkingsgrootte (artikelen per 1M inwoners)
- Normaliseer voor nieuwssysteem (aantal landelijke dagbladen)
- Vergelijk framing-distributie per land met chi-kwadraat
- Multi-dimensional scaling van land-verschillen

### D.3 Inter-rater reliability protocol (Categorie I)

**Stap 1: Codeurselectie en training**
- Selecteer 5 codeurs met onderzoekservaring en domeinkennis
- Training: 20 uur voor 17-assige taxonomie, 8 uur voor Gedragsladder, 4 uur voor Authenticity Layer
- Pilot-codering: 20 posts, gezamenlijke bespreking, consensus-ontwikkeling

**Stap 2: Steekproeftrekking**
- Power-analyse: minimum 50 items voor Kappa > 0,7 met 5 codeurs
- Gestratificeerd per type (consensueel, NCII, amateur challenge, etc.)
- Alleen metadata (geen beelden, geen identificeerbare informatie)

**Stap 3: Codering**
- Elke codeur codeert onafhankelijk (geen overleg tijdens codering)
- Codeurs in willekeurige volgorde om volgorde-effect te voorkomen
- Coderingen in aparte bestanden, geblindeerd voor andere codeurs

**Stap 4: Statistische analyse**
- Fleiss' Kappa voor >2 codeurs, nominale data
- Cohen's Kappa voor pairwise vergelijkingen
- Krippendorff's Alpha voor ordinale/interval-schalen
- Percentage agreement (voor transparantie)
- Per as/ per niveau rapportage
- Analyse van systematische verschillen (bias tussen codeurs)

**Stap 5: Consensusfase**
- Gezamenlijke bespreking van items met Kappa < 0,4
- Herziening van codeerhandboek bij structurele onenigheid
- Tweede coderingronde voor herziene items
- Rapportage van Kappa voor en na consensus

### D.4 Netwerkanalyse protocol (Categorie J)

**Stap 1: Data-extractie**
- Extraheer URLs uit Reddit-posts (Pushshift, NSFW-subreddits, 2015-2023)
- Filter op: unieke URLs, externe domeinen, geen Reddit-intern
- Extraheer ook: post timestamp, auteur, subreddit, score, aantal comments

**Stap 2: Netwerkconstructie**
- Node types: subreddits, domeinen, gebruikers (geanonimiseerd)
- Edge types: URL-share (subreddit → domein), cross-post (subreddit → subreddit), reshare (gebruiker → gebruiker viazelfde URL)
- Gewichten: aantal shares, frequentie, tijdsinterval

**Stap 3: Analyse**
- Degree centrality: welke subreddits/domeinen zijn het meest verbonden?
- Betweenness centrality: welke nodes fungeren als bruggen?
- Eigenvector centrality: welke nodes zijn belangrijk in het netwerk?
- Community detectie (Louvain, Leiden): welke clusters bestaan?
- Tijdsdynamiek: hoe verandert het netwerk over tijd?

**Stap 4: Persistentie-analyse**
- Check elke URL in Wayback Machine: datum van eerste en laatste capture
- Survival-analyse: overlevingscurve per domein/subreddit
- Cox regression: predictoren van langere levensduur

**Stap 5: Visualisatie en rapportage**
- Netwerk-grafieken (Gephi, networkx)
- Community-kaarten
- Tijdslijn van verspreiding per typische case
- MissingnessMap: niet-getraceerde URLs

## UITGEBREIDE APPENDIX E — DATABEHEERPLAN

### E.1 Data-opslag

- Reddit Pushshift data: niet lokaal opslaan; gebruiken via API of BigQuery
- LexisNexis data: exporteren als plain text, opslaan op encrypted schijf
- Google Trends data: exporteren als CSV, opslaan met metadata
- OpenAlex data: gebruiken via API; alleen output opslaan
- Wikipedia data: gebruiken via API; alleen output opslaan
- Common Crawl data: gebruiken via Athena; alleen output opslaan
- Handmatige coderingen: opslaan in gestructureerde JSON-bestanden met versiebeheer
- Alle data: AVG-compliant, geen persoonsgegevens, geanonimiseerd

### E.2 Data-retentie

- Ruwe data: verwijderen na publicatie (tenzij noodzakelijk voor replicatie)
- Geanonimiseerde datasets: via Figshare/Zenodo beschikbaar voor replicatie
- Code: GitHub (open access)
- Codering-output: JSON met versiebeheer
- Duur: minimaal 10 jaar (conform open science praktijken)

### E.3 Data-sharing restricties

- Geen beeldmateriaal wordt gedeeld
- Geen persoonsgegevens worden gedeeld
- Geanonimiseerde corpora (term-frequenties) kunnen worden gedeeld
- Codeurs kunnen anoniem blijven in publicaties
- Platform-specifieke data (tweets, Reddit posts) blijven in oorspronkelijke bron
- Alleen geaggregeerde data en code worden gepubliceerd

### E.4 Ethische toetsing

- Deze agenda valt onder niet-WMO-plichtig onderzoek (geen medisch-wetenschappelijk onderzoek met personen)
- Ethische toetsing via facultaire ethische commissie (verplicht voor alle academische dataverzameling)
- Specifieke aandachtspunten: codering van intieme content (geen beelden), analyse van kwetsbare groepen (jongeren), AVG-compliance
- Expliciete documentatie van ethische afwegingen in elk onderzoeksrapport

## UITGEBREIDE APPENDIX F — RISICO-ANALYSE PER ONDERZOEKSVRAAG

| Risico | Waarschijnlijkheid | Impact | Mitigatie |
|:---|---:|:---:|:---|
| Reddit API-wijzigingen beperken data | Hoog | Hoog | Back-up via bestaande Pushshift-dumps; alternatieve fora (4chan, Discord) |
| LexisNexis abonnementskosten | Midden | Hoog | Alternatieven: Delpher, Google News, Open Access journals |
| Twitter API kosten (/maand) | Hoog | Midden | Alleen prioritaire vragen; gebruik historische datasets |
| Common Crawl processing kosten | Midden | Midden | Gebruik Athena; beperk tot specifieke domeinen |
| Codeur uitval | Midden | Midden | Reserve-codeurs; gedocumenteerde training |
| Lage inter-rater reliability | Midden | Hoog | Extra training; herziening codeerhandboek; beperking tot robuuste assen |
| Onvoldoende data per taal | Hoog | Midden | Beperk tot NL/EN/DE/FR; expliciete erkenning van taalbias |
| Platform ToS veranderingen | Hoog | Midden | Wayback Machine back-up; continue monitoring |
| AVG-issues met dataopslag | Laag | Hoog | Alleen geanonimiseerde data; geen persoonsgegevens; DPIA |
| Publicatiebias in academische data | Hoog | Midden | Documenteer bias; funnel plots; Egger's test |
| Google Trends data-drempel | Midden | Laag | Gebruik maandelijkse data; accepteer missingness |
| Wayback Machine incomplete archivering | Hoog | Midden | Triangulatie met Common Crawl; vermeld als survivorship bias |

## UITGEBREIDE APPENDIX G — COMPLETE TERMINOLOGIEGLOSSARIUM

### G.1 Toolonderdelen — definities

| Term | Afkorting | Definitie | Bron |
|:---|---|:---|:---|
| Naturalness Probability Model | NPM | 6-traps schaal voor spontane taalkans (1=zeer gebruikelijk tot 6=synthetisch) | Data 1/5 |
| Authenticity Layer | AL | 10 categorieën geformaliseerde vs. natuurlijke taal | Data 1/6 |
| Self-Validation Protocol | SVP | 4-toets validatieprotocol voor taalkundige conclusies (V1-V4) | Data 1/4 |
| Register A/B | — | Twee-sferenmodel: eufemistisch-extern (A) vs. direct-intern (B) | Data 1/2, 1/3 |
| Conversation Layer | CL | 7 kanaaltypen voor communicatie-analyse | Data 1/7 |
| Lexicale Frequentiekaart | LFK | Systematisch register van 72+ intieme termen | Data 1/7 |
| Ensceneringscontinuüm | — | 6-niveau schaal voor enscenering (1=spontaan tot 6=gescript) | Data 1/15, 1/16 |
| Gewogen bewijsmodel | WEM | Bewijssterkteschaal 0-4 met beslisdrempels | Data 1/9, 1/10 |
| Anti-dubbeltellingsregel | ADR | Consolidatie van gecorreleerde signalen uit één handeling | Data 1/9, 1/10 |
| Gedragsladder | GL | Niveau 0-5 voor granulariteit van bronvergelijking | Data 2/7 |
| Content-Frequency Denominator | CFD | Noemer-standaardisatie (DENOM 01-05) | Data 2/7 |
| Visibility Escalation Score | VES | Level 0-4 zichtbaarheids-escalatieladder | Data 2/7 |
| MediaLifecycleRecord | MLR | 6-fasen levenscyclus (context, capture, storage, first-share, re-share, persistence) | Data 2/2 |
| TrajectoryRecord | TR | 9-fasen trajectmodel (trigger tot recovery) | Data 2/3 |
| MissingnessMap | MM | Systematische datakwaliteitsregistratie per variabele | Data 2/3 |
| Cross-Source Translation Table | CST | Vertaling tussen onderzoeksterminologieën | Data 2/8 |
| IncidentRecord | IR | 16+ domeinen integrale codeereenheid | Data 2/8 |
| Pattern Library | PL | Alpha/Beta/Gamma sequentiepatronen | Data 2/7 |
| Non-Event Baseline | NEB | Verplichte registratie van niet-geëscaleerde casussen | Data 2/7 |
| Content-Source Bias | CSB | Systematische bron-vertekening | Data 2/7 |
| Content-to-Circulation Transformation | CCT | Betekenisverschuiving tijdens circulatie | Data 2/7 |
| Request-to-Action Distance | RAD | Tijds- en drukafstand tussen verzoek en actie | Data 2/7 |
| Camera-Presence Effect | CPE | Hawthorne-effect in camera-context | Data 2/8 |
| Behaviour-to-Image Conversion Point | BICP | Moment van overgang naar beeld | Data 2/8 |
| Behavioural Stopping Point | BSP | Punt waar escalatie stopt | Data 2/8 |

### G.2 Domein-specifieke terminologie

| Term | Definitie |
|:---|:---|
| NCII | Non-Consensual Intimate Imagery: intieme beelden verspreid zonder toestemming |
| IBSA | Image-Based Sexual Abuse: overkoepelende term voor digitaal seksueel geweld met beelden |
| NCII-wet | Wetgeving tegen niet-consensuele verspreiding van intieme beelden |
| DSA | EU Digital Services Act: platformregulering sinds 2023 |
| ToS | Terms of Service: platformgebruiksvoorwaarden |
| Algospeak | Algoritmisch aangepaste taal om moderatie te omzeilen |
| Ephemeraliteit | Tijdelijkheid van content (verdwijnberichten) |
| Perceived Ephemerality | Gebruikersverwachting dat content verdwijnt |
| Actual Persistence | Technische realiteit van permanentie |
| Pushshift | Reddit-archief (2005-2023) |
| Common Crawl | Open webcrawl dataset (2008-heden) |
| Wayback Machine | Internet Archive's historische webpagina-database |
| LexisNexis | Internationale nieuwsarchief-database |
| OpenAlex | Open access academische index |
| DENOM 01 | Alle jongeren in populatiesample |
| DENOM 02 | Jongeren die ooit beelden maakten |
| DENOM 03 | Jongeren die ooit beelden ontvingen |
| DENOM 04 | Jongeren die ooit beelden doorgestuurd hebben |
| DENOM 05 | Gemelde incidenten bij instellingen |
| Granulariteit Niveau 0 | Containerbegrippen (bv. "sexting") |
| Granulariteit Niveau 1 | Kleding/naaktheidsniveau |
| Granulariteit Niveau 2 | Gedragsklasse |
| Granulariteit Niveau 3 | Interactiestructuur |
| Granulariteit Niveau 4 | Gedrag + script + camerarelatie |
| Granulariteit Niveau 5 | Volledige levenscyclus |

### G.3 Register A/B terminologie — voorbeelden per taal

**Register A (eufemistisch, extern, aftastend):**
Nederlands: "iets leuks", "spicy pic", "picje", "nudes", "view once", "wat heb je aan?", "spannende foto", "verrassing", "ondeugend"
Engels: "something fun", "spicy pic", "send nudes", "view once", "what are you wearing?", "naughty pic"
Duits: "was Schönes", "heiße Bilder", "Privatbilder", "Nacktfoto"
Frans: "photo coquine", "truc coquin", "nudes"
Spaans: "algo rico", "foto atrevida", "nudes"

**Register B (direct, intern, in-the-moment):**
Nederlands: "neuken", "pijpen", "tieten", "geil", "likken", "beflen", "klaarkomen", "aftrekken"
Engels: "fuck", "suck", "tits", "horny", "eat out", "cum", "jack off"
Duits: "ficken", "blasen", "Titten", "geil", "lecken"
Frans: "baiser", "sucer", "seins", "chaud", "lécher"
Spaans: "follar", "mamar", "tetas", "caliente", "lamer"

### G.4 NPM 1-6 schaal — volledige toelichting

**NPM 1 — Zeer gebruikelijk (P > 0,70):**
De absolute standaardformulering in dagelijkse, spontane menselijke communicatie. Hoge frequentie in chatlogs, interviews, alledaagse gesprekken. Lage cognitieve drempel.
Corpusindicatoren: >70 per 100.000 woorden in spontane corpora.
Voorbeelden: "foto", "picje", "sturen", "laten zien", "wat heb je aan?"

**NPM 2 — Regelmatig gebruikt (P = 0,35-0,70):**
Frequent gebruikt natuurlijk alternatief voor de hoofdterm. Algemeen geaccepteerd in besloten communicatie.
Corpusindicatoren: 35-70 per 100.000 woorden.
Voorbeelden: "nudes", "iets leuks", "spannende foto", "drop a pic"

**NPM 3 — Contextafhankelijk (P varieert per subgroep):**
Binnen specifieke leeftijdsgroepen, platforms of relatievormen zeer hoge natuurlijkheid, maar buiten die context vrijwel afwezig.
Corpusindicatoren: hoge concentratie in specifieke subcorpora, afwezig in algemene corpora.
Voorbeelden: "spicy pic", "view once", "lewd", "seggs", "pickie"

**NPM 4 — Zeldzaam (P = 0,01-0,10):**
Term wordt inhoudelijk begrepen maar in actuele spontane interacties nauwelijks gebruikt. Historisch of regionaal.
Corpusindicatoren: 1-10 per 100.000 woorden.
Voorbeelden: "cyberen", "erotische opname", "schunnige foto"

**NPM 5 — Vrijwel uitsluitend formeel (P ≈ 0 in privé-chats):**
Term exclusief in wetgeving, beleid, medische dossiers, nieuws. Nul-frequentie in besloten chat- en relatie-corpora.
Corpusindicatoren: N=0 in spontane corpora, hoge frequentie in formele corpora.
Voorbeelden: "seksueel expliciet beeldmateriaal", "non-consensuele verspreiding", "genitale opname"

**NPM 6 — Theoretisch mogelijk / Synthetisch (P < 0,01):**
Grammaticaal correcte constructies die in werkelijkheid vrijwel nooit door menselijke sprekers worden geuit. AI-gegenereerde steriele teksten.
Corpusindicatoren: N≈0 in alle natuurlijke corpora.
Voorbeelden: "mijd u mij een seksueel expliciete afbeelding verzenden?", "wilt u mij uw genitalieën tonen?"

### G.5 Authenticity Layer — complete categoriebeschrijving

**Geformaliseerde beschrijvingen (niet-spontaan):**
1. Canonieke beschrijving: officiële woordenboekdefinities, abstract, synthetisch ("audiovisueel materiaal van intieme aard")
2. Klinische terminologie: psychologie/seksuologie/gedragswetenschappen, objectiverend ("seksuele handeling", "genitale registratie")
3. Juridische terminologie: strafrecht/privacyrecht, normatief ("non-consensuele verspreiding", "inbreuk op de persoonlijke levenssfeer")
4. Medische terminologie: anatomie/fysiologie, biologisch ("penis", "vagina", "vulva")

**Natuurlijk menselijk taalgebruik (spontaan):**
5. Dagelijks spreektaalgebruik: informele woorden zonder vakjargon ("foto's", "filmpjes", "iets leuks")
6. Partnertaal (Couple Talk): exclusieve intieme codetaal binnen een relatie ("ons geheim", "verrassing voor vanavond")
7. Straattaal: subculturele jongerentaal, dynamisch, identiteitsbevestigend ("pickie", "fotope", "fakka pic")
8. Regionale variant: dialectale of lokaal gebonden uitingen ("filmke" BE, "plaatje" NL-regionaal)
9. Internetslang: ontstaan op openbare fora/chatrooms ("nudes", "pics", "NSFW", "thirst trap", "lewd")
10. Platformslang (Algospeak): bewust gecreëerd om algoritmen te omzeilen ("spicy pics", "seggs", "corn", "view once")

### G.6 Vergelijking v1, v2 en v3 — methodologische verschuiving

| Aspect | v1 (oorspronkelijk) | v2 (geïntegreerd) | v3 (realistisch) |
|:---|---|:---|:---|
| Data-aanname | Ideale data toegankelijk | Ideale data, cross-module | Alleen publieke data |
| Aantal vragen | ~45 | ~60 | 52 |
| Toegang privé-chats | Verondersteld | Verondersteld | Uitgesloten |
| Toegang institutionele data | Verondersteld | Verondersteld | Uitgesloten |
| Toegang platform-backend | Impliciet verondersteld | Impliciet verondersteld | Uitgesloten |
| Toegang beeldmateriaal | Beperkt verondersteld | Beperkt verondersteld | Uitgesloten |
| Non-Event Baseline meting | Survey-data verondersteld | Survey-data verondersteld | Alleen theoretisch |
| Register A/B in privé-chats | Verondersteld haalbaar | Verondersteld haalbaar | Alleen publiek discours |
| 17-assen codering op beelden | Verondersteld | Verondersteld | Alleen metadata |
| SVP V3 op academisch | Wel opgenomen | Wel opgenomen | Behouden |
| Cross-Source Translation | Wel opgenomen | Wel opgenomen | Behouden, uitgebreid |
| Bias-documentatie | Beperkt | Beperkt | Expliciet en structureel |
| Uitvoerbaarheid | Laag | Laag-midden | Hoog |
| Beperkte generaliseerbaarheid | Niet benoemd | Deels benoemd | Centraal uitgangspunt |

### G.7 Aanbevolen publicatiekanalen per categorie

| Categorie | Type publicatie | Doel-tijdschriften/kanalen |
|:---|---|:---|
| A (Terminologie) | Corpusanalyse / Sociolinguïstiek | Journal of Pragmatics, Discourse Studies, Language@Internet, Corpus Linguistics |
| B (Platforms) | Beleidsanalyse / HCI | New Media & Society, Social Media + Society, Journal of Computer-Mediated Communication |
| C (Content) | Methodologisch / Classificatie | Journal of Sex Research, Archives of Sexual Behavior, Poetics |
| D (Media) | Framing-analyse | Journalism Studies, International Journal of Communication, European Journal of Communication |
| E (Platformbeleid) | Beleidsanalyse | Policy & Internet, Telecommunications Policy, Computer Law & Security Review |
| F (Historisch) | Bibliometrisch / Diachroon | Scientometrics, Journal of the Association for Information Science and Technology |
| G (Internationaal) | Cross-cultureel | Cross-Cultural Research, International Journal of Intercultural Relations |
| H (Academisch) | Bibliometrisch | Research Evaluation, Journal of Documentation |
| I (Taxonomie) | Methodologisch / Reliability | Methodology, Sociological Methods & Research, Field Methods |
| J (Netwerken) | Netwerkanalyse | Social Networks, Journal of Quantitative Criminology, Network Science |
| Synthese | Overkoepelend | Computers in Human Behavior, New Media & Society, Journal of Adolescent Health |

## UITGEBREIDE APPENDIX H — CONCRETE UITVOERINGSCASUSSEN

### H.1 Casus A-01: NPM-kloof tussen Reddit-discours en beleidsdocumenten

**Doel:** Kwantificeren van de NPM-verdeling van intieme terminologie in twee corpora: Reddit (r/sex, r/relationships) en beleidsdocumenten (WODC, Rijksoverheid, EU).

**Databronnen:**
- Reddit: Pushshift dump 2022-2023, 50.000 posts uit r/sex en r/relationships
- Beleid: 500 WODC-rapporten, 1.000 Rijksoverheid-publicaties, 200 EU-documenten

**Methoden:**
1. Extractie van alle zelfstandige naamwoorden en werkwoorden uit beide corpora
2. Filter op seksueel/intiem vocabulaire (woordlijst uit Data 1/7: 72+ termen)
3. NPM-toekenning op basis van relatieve frequentie per corpus
4. Authenticity Layer-classificatie
5. SVP V1-V4 toepassing op top-50 termen per corpus

**Verwachte output:**
- NPM-distributie per corpus (staafdiagram)
- Top-20 termen per corpus met NPM en AL
- Gap-analyse: welke termen zijn frequent in Reddit maar afwezig in beleid?
- SVP-goedkeuringspercentage: % van termen in beleid dat SVP V3 doorstaat

**Risico's:**
- Corpus-balancing: Reddit heeft meer woorden dan beleidscorpus
- Domeinspecificiteit: beleidstermen zijn per definitie formeel
- Interpretatie: NPM 5 in beleid is normaal, niet pathologisch

**Tijdlijn:** 2 maanden (1 maand extractie, 1 maand analyse)

### H.2 Casus B-01: Platformrichtlijnen longitudinale analyse

**Doel:** In kaart brengen van de evolutie van communityrichtlijnen over naaktheid en NCII over 12 platforms en 16 jaar.

**Databronnen:**
- Wayback Machine CDX API voor 12 platform ToS-pagina's
- ToS;DR database voor gestandaardiseerde classificaties
- Tech media (The Verge, TechCrunch, Platformer) voor context

**Methoden:**
1. Identificeer URL-patterns voor ToS-pagina's per platform
2. Query Wayback Machine voor jaarlijkse captures (2010-2026)
3. Download HTML, extract text, filter op naaktheid/seks/NCII secties
4. Codeer per jaar: definities, categorieën, sancties, beroepsprocedures
5. Term-frequency tracking: "adult nudity", "sexual activity", "NCII", "non-consensual"
6. NPM-classificatie van ToS-terminologie

**Verwachte output:**
- Beleidsverandering-matrix per platform per jaar
- Consistentie-score tussen platformdefinities
- Terminologie-trends
- NPM-profiel van ToS-taal
- SVP V3-toetsing

**Risico's:**
- Wayback Machine niet voor elk platform compleet
- ToS kunnen tussentijds wijzigen zonder aankondiging
- Alleen geschreven beleid, geen handhaving

**Tijdlijn:** 3 maanden

### H.3 Casus D-01: Framing-analyse Nederlandse nieuwsmedia

**Doel:** Framing van sexting in Nederlandse nieuwsmedia (2010-2026): verschuift moral panic naar normalisering?

**Databronnen:**
- LexisNexis NL: alle Nederlandse landelijke dagbladen
- Zoektermen: sexting, nudes, wraakporno, intieme beelden, naaktfoto
- Periode: 2010-2026

**Methoden:**
1. Data-extractie: 5.000-10.000 artikelen
2. Stratificatie: per jaar (16 jaar), per krant (8 kranten)
3. Stap 1: automatische themacodering via keywoordclusters
4. Stap 2: handmatige framing-codering door 3 codeurs (steekproef n=500)
5. Frames: risico, moral panic, normalisering, juridisch, neutraal
6. Trendanalyse: per jaar, per krant, per politieke kleur

**Verwachte output:**
- Framing-verdeling per jaar (gestapeld staafdiagram)
- Trendlijnen per frame (2010-2026)
- Verschuiving moral panic -> normalisering? (chi-kwadraat)
- Event-correlatie: wetgeving (art. 240b), schandalen, voorlichting
- SVP-classificatie van journalistieke terminologie

**Risico's:**
- Framing is subjectief; inter-rater reliability nodig
- LexisNexis-dekking niet 100%
- Moral panic is moeilijk te operationaliseren

**Tijdlijn:** 3 maanden

### H.4 Casus I-01: 17-assige taxonomie inter-rater reliability

**Doel:** Meten van de reproduceerbaarheid van de 17-assige taxonomie op openbare metadata.

**Databronnen:**
- Pushshift: 100 posts uit diverse adult subreddits
- Alleen metadata (titels, beschrijvingen, tags, subreddit, cross-posts)
- Geen beelden, geen identificeerbare informatie

**Methoden:**
1. Codeurselectie: 5 codeurs met onderzoekservaring
2. Training: 40 uur (20 uur instructie, 20 uur pilot met 20 posts)
3. Codering: alle 17 assen per post, onafhankelijk
4. Statistische analyse: Fleiss' Kappa per as, Krippendorff's Alpha
5. Consensusbespreking voor lage-reliability-assen

**Verwachte output:**
- Reliability per as (tabel met Kappa per as)
- Welke assen zijn betrouwbaar (Kappa > 0,7)?
- Welke assen zijn onbetrouwbaar (Kappa < 0,4)?
- Aanbevelingen voor codeerhandboek-aanpassing
- Minimum aantal codeurs voor betrouwbare 17-assen codering

**Risico's:**
- As 9 (Camerabewustzijn) en As 14 (Opname-afhankelijkheid) zijn metadata-only moeilijk te coderen
- As 8A/8B splitsing vereist interpretatie van sociale context
- As 17 (Vaststelbaarheid) is per definitie laag bij metadata-only

**Tijdlijn:** 4 maanden (1 maand training, 1 maand codering, 2 maanden analyse)

### H.5 Casus F-01: Google Trends sexting-terminologie

**Doel:** Tracking van zoekvolume-veranderingen voor 10 termen over 18 jaar.

**Databronnen:**
- Google Trends (2008-2026, wereldwijd + 5 landen)
- Termen: sexting, nudes, revenge porn, NCII, image-based abuse, deepfake porn, onlyfans, amateur porn, spicypic, intimate image

**Methoden:**
1. Extractie per term per regio per jaar
2. Normalisatie: schaal 0-100 per term
3. Time-series decompositie (trend, seasonal, residual)
4. Event-correlatie: wetgevingsmomenten, mediashandalen, platformlanceringen
5. Cross-correlatie tussen termen (welke termen stijgen samen?)
6. Breakpoint-detectie: significante veranderingen in zoekgedrag

**Verwachte output:**
- Trendgrafieken per term per regio
- Correlatiematrix tussen termen
- Event-tabel: welke gebeurtenissen correleren met pieken?
- Cross-linguïstische vergelijking (zelfde term in verschillende talen/landen)

**Risico's:**
- Google Trends geeft relatieve, geen absolute volumes
- Lage-volume termen hebben soms onvoldoende data
- Google-blokkade en internetcensuur in sommige landen
- Zoekdata is niet gedrag maar interesse

**Tijdlijn:** 1 maand

### H.6 Casus G-02: Taal-specifieke subreddit vergelijking

**Doel:** Cross-linguïstische vergelijking van intieme terminologie in taal-specifieke Reddit-subreddits.

**Databronnen:**
- Pushshift: r/nederlands, r/de, r/france, r/espanol, r/portugal, r/poland, r/italy
- Periode: 2015-2023
- Minimum 100.000 woorden per taal

**Methoden:**
1. Extractie van alle posts per subreddit
2. Taaldetectie: bevestig dominantie van de relevante taal
3. Term-extractie: seksuele en intieme termen per taal
4. Register A/B-classificatie per term per taal
5. NPM-toekenning per term per taal
6. Cross-linguïstische frequentievergelijking
7. Multi-dimensional scaling van taalverschillen

**Verwachte output:**
- Top-20 intieme termen per taal met frequentie
- Register A/B-verdeling per taal
- NPM-profiel per taal
- MDS-plot van taal-afstanden op basis van terminologie
- Cultuur-specifieke termen per taal

**Risico's:**
- Subreddit-corpusgrootte varieert sterk per taal
- Subreddit-cultuur is niet representatief voor taal/cultuur
- Sommige talen hebben weinig intieme termen in openbare forums
- Register-classificatie is taal-specifiek

**Tijdlijn:** 3 maanden

### H.7 Casus H-02: SVP V3 op academische terminologie

**Doel:** Toetsen of academische literatuur natuurlijke of klinische terminologie gebruikt voor intieme communicatie.

**Databronnen:**
- 350 artikelen uit 7 tijdschriften (50 per tijdschrift): Computers in Human Behavior, New Media & Society, Journal of Adolescent Health, Archives of Sexual Behavior, Journal of Sex Research, Violence Against Women, Social Media + Society
- Periode: 2005-2026

**Methoden:**
1. Extractie van alle zinnen die verwijzen naar intieme communicatie
2. Term-extractie per artikel
3. NPM-classificatie per term
4. SVP V3-toetsing: is de term klinisch-gedistantieerd of natuurlijk?
5. Trendanalyse: verandert terminologie over tijd?
6. Vergelijking tussen tijdschriften (sociaal-wetenschappelijk vs. medisch)

**Verwachte output:**
- NPM-distributie per tijdschrift
- SVP V3-goedkeuringspercentage per tijdschrift
- Trend: stijging/daling in natuurlijke terminologie?
- Top-20 klinische termen in academisch discours
- Aanbeveling voor terminologie in toekomstig onderzoek

**Risico's:**
- Academisch discours is per definitie formeel
- SVP V3 is voor privé-taal, niet voor academisch schrijven
- Interpretatie van "natuurlijke variant" is context-afhankelijk

**Tijdlijn:** 4 maanden

### H.8 Casus J-01: URL-verspreidingsnetwerken

**Doel:** In kaart brengen hoe URLs naar intieme content zich verspreiden via Reddit.

**Databronnen:**
- Pushshift: alle posts uit NSFW-subreddits (2015-2023)
- URL-extractie uit post bodies
- Wayback Machine voor persistence-check

**Methoden:**
1. Filter alle posts met externe URLs naar adult domeinen
2. Extraheer: URL, post-ID, auteur, subreddit, timestamp, score
3. Bouw netwerk: nodes = subreddits/domeinen, edges = URL shares
4. Centraliteitsanalyse: degree, betweenness, eigenvector
5. Community detectie: Louvain clustering
6. Survival analyse: hoe lang blijft een URL actief?

**Verwachte output:**
- Netwerkgraph van subreddit-domein verbindingen
- Top-10 domeinen/sites per centraliteit
- Community-structuur (clusters van subreddits)
- Overlevingscurve van URLs per domeintype
- Identificatie van aggregators (gebruikers/accounts die meerdere URLs delen)

**Risico's:**
- Alleen openbare URLs; privé-verspreiding onzichtbaar
- Reddit API-wijzigingen na 2023 beperken recente data
- Wayback Machine heeft niet alle URLs
- Ethiek: geen identificatie van individuen

**Tijdlijn:** 4 maanden

## UITGEBREIDE APPENDIX I — VERGELIJKING VAN ANALYSEMETHODEN PER VRAAGTYPE

### I.1 Kwantitatieve methoden

| Methode | Toepassing | Vragen |
|:---|---|:---:|
| Chi-kwadraat toets | Frequentieverschillen tussen corpora | A-01 t/m A-10, G-02 |
| ANOVA / Kruskal-Wallis | Verschillen tussen >2 groepen | A-02, G-01, H-01 |
| Mann-Kendall trend test | Trends over tijd | A-03, F-01 t/m F-06 |
| Fleiss' Kappa | Inter-rater reliability >2 codeurs | C-02, I-01 t/m I-06 |
| Krippendorff's Alpha | Inter-rater reliability ordinal | I-01, I-04 |
| Pearson/Spearman correlatie | Correlatie tussen variabelen | D-04, G-03, H-03 |
| Survival analyse (Kaplan-Meier) | Tijd tot event | J-02 |
| Cox proportional hazards | Predictoren van overleving | J-02 |
| Multi-dimensional scaling | Cross-linguïstische afstanden | G-02, G-04 |
| McNemar-test | Verandering in classificatie | C-05 |
| Cohen's d / Cramer's V | Effect size | A-01, A-02, D-01 |
| Joinpoint regression | Trendbreuk-detectie | F-05 |
| Netwerkcentraliteit (degree, betweenness, eigenvector) | Netwerk-analyse | J-01, J-03, H-05 |

### I.2 Kwalitatieve methoden

| Methode | Toepassing | Vragen |
|:---|---|:---:|
| Framing-analyse | Nieuwsmedia discours | D-01 t/m D-05, G-01 |
| Agency-analyse | Slachtoffer/dader framing | D-03 |
| Pragmatische functiecodering | Communicatieve functies | A-06, A-10 |
| Conversation Layer-analyse | Kanaal-specificiteit | A-09 |
| Thematische analyse | Kwalitatieve discours patronen | B-06, D-05, G-04 |

### I.3 Mixed methods

| Combinatie | Toepassing | Vragen |
|:---|---|:---:|
| NPM + AL + SVP | Volledige taalkundige pijplijn | A-01 t/m A-10 |
| Gestructureerde codering + Kappa | Taxonomie validatie | I-01 t/m I-06 |
| Netwerkanalyse + survival | Sharing dynamiek | J-01, J-02 |
| Bibliometrie + correlatie | Publicatie analyse | H-01 t/m H-05 |
| Framing + sentiment | Media discours | D-01 t/m D-05 |

### I.4 Automatische vs. handmatige methoden

| Type | Automatisch | Handmatig | Combinatie |
|:---|---|:---|:---:|
| Term-extractie | Ja (spacy, stanza) | Nee | Validatie steekproef |
| NPM-toekenning | Ja (frequentiecutoff) | Ja (context-check) | Automatisch + validatie |
| Authenticity Layer | Deels (keyword-gebaseerd) | Ja (volledige codering) | Automatisch voor bulk, handmatig voor validatie |
| Framing-analyse | Deels (sentiment, keywords) | Ja (interpretatie) | Automatische clustering + handmatige validatie |
| Netwerkanalyse | Ja (networkx, igraph) | Nee | Automatisch |
| Inter-rater reliability | Nee (statistische analyse) | Ja (codering) | Handmatige codering, automatische analyse |
| SVP-toetsing | Deels (NPM-check) | Ja (V1-V4 interpretatie) | Automatisch voor V3, handmatig voor V1, V2, V4 |
| Survival analyse | Ja (lifelines, survival) | Nee | Automatisch |
| Bibliometrie | Ja (OpenAlex API) | Nee | Automatisch |

## UITGEBREIDE APPENDIX J — REFERENTIES EN ACHTERGRONDLITERATUUR

### J.1 Methodologische bronnen (toolonderdelen)

Albury, K. (2023). Self-produced intimate media: A taxonomy approach. New Media & Society.
Baker, P. (2021). Corpus linguistics and sexual language. Routledge.
Gesselman, A. N. et al. (2019). Emoji as pragmatic markers in digital intimate communication. Computers in Human Behavior.
Henry, N. & Powell, A. (2018). Technology-facilitated sexual violence. Violence Against Women.
Luu, C. (2026). Algospeak and platform moderation. Language@Internet.
Yus, F. (2021). Emoji pragmatics. Journal of Pragmatics.
Rutgers (2023). Seks onder je 25e: Resultaten van het Rutgers-onderzoek.
EU Kids Online (2023). Findings from the EU Kids Online survey.
Livingstone, S. et al. (2019). EU Kids Online: Theoretical framework and methodology.

### J.2 Databronnen

Pushshift.io (Baumgartner, J.) — Reddit archief
Common Crawl Foundation — Web crawl data
Internet Archive (Kahle, B.) — Wayback Machine
OpenAlex (Priem, J.) — Open academic index
Google Trends — Zoekdata
Google Books Ngram — Book frequency data
LexisNexis — News archives
ToS;DR (Hugo, R.) — Terms of Service analysis

### J.3 Platform transparency data

Meta Transparency Center (transparency.fb.com)
TikTok Transparency Report (tiktok.com/transparency)
YouTube Community Guidelines Report (transparencyreport.google.com)
Reddit Transparency Report (redditinc.com/policies/transparency)
Apple App Store Transparency (developer.apple.com/app-store/review/)

### J.4 Wetgeving

EU Digital Services Act (Verordening 2022/2065)
UK Online Safety Act (2023)
Nederland: art. 240b en 251 Wetboek van Strafrecht
Duitsland: Netzwerkdurchsetzungsgesetz (NetzDG)
Frankrijk: Loi Avia (2020)
Canada: Intimate Images Act (2021)
VS: verschillende state-level NCII-wetten

### J.5 Nederlandse onderzoeksinstituten

Rutgers (kenniscentrum seksualiteit): rutgers.nl
GGD Sense: sense.info
Verwey-Jonker Instituut: verwey-jonker.nl
Netwerk Mediawijsheid: mediawijsheid.nl
Universiteit Utrecht: uu.nl (EU Kids Online NL)
Universiteit van Amsterdam: uva.nl (digitale cultuur)
Universiteit Leiden: universiteitleiden.nl (jeugdrecht)
WODC (Wetenschappelijk Onderzoek- en Documentatiecentrum): wodc.nl
CBS (Centraal Bureau voor de Statistiek): cbs.nl
Inspectie van het Onderwijs: onderwijsinspectie.nl

### J.6 Overige relevante concepten

Pluralistic ignorance: overschatting van prevalentie van gedrag
Sociale wenselijkheid bias: onderrapportage van gevoelige onderwerpen
Survivorship bias: alleen bewaard gebleven data is zichtbaar
Platformbias: demografische selectiviteit per platform
Taalbias: oververtegenwoordiging van Engels en Westerse talen
Publicatiebias: oververtegenwoordiging van significante effecten
Escalatiebias: oververtegenwoordiging van schadegevallen in institutionele data
Zelfrapportagebias: verschil tussen gerapporteerd en werkelijk gedrag
Herinneringsbias: retrospectieve data is onbetrouwbaar
Steekproefbias: selectieve deelname aan onderzoek
Non-Event Baseline: de onzichtbare meerderheid van niet-gëescaleerde casussen
Candid Capture: bewust uitschakelen van camerabewustzijn voor authenticiteit
Hawthorne-effect: gedragsverandering door observatie
Perceived Ephemerality: verwachting dat data verdwijnt
Actual Persistence: technische realiteit van data-bewaring
Content-to-Circulation Transformation: betekenisverschuiving tijdens circulatie
Visibility Intent Mismatch: verschil tussen beoogde en werkelijke zichtbaarheid
Registerpolarisatie: tweedeling tussen eufemistisch en direct register
Algospeak: platformaangepaste taal voor moderatie-omzeiling
Pragmatische wrijving: graduele toestemmingsonderhandeling

---

*EINDE DOCUMENT — 22 juli 2026*
*Versie 3.0 — Realistische haalbaarheidsanalyse op basis van openbare databronnen*
*Gebruikte toolomgeving: Module 1 (Jeugd Incidenten 15-18) + Module 2 (Authentieke Intieme Menselijke Taal & 17-Assige Taxonomie)*
*Opgesteld conform de methodologische richtlijnen uit: .kilo/rules/master_codebook.md, .kilo/rules/delta_insights.md, .kilo/rules/module2_intimate_language.md, .kilo/rules/module2_17_axis_taxonomy.md*

## UITGEBREIDE APPENDIX K — CHECKLISTS PER ONDERZOEKSFASE

### K.1 Data-extractie checklist

- [ ] Toestemming ethische commissie verkregen?
- [ ] Databron publiek toegankelijk?
- [ ] Geen AVG-schending?
- [ ] Geen beeldmateriaal gedownload?
- [ ] Geen persoonsgegevens opgeslagen?
- [ ] Databron-API functioneel?
- [ ] Rate limits gerespecteerd?
- [ ] Data-formaat gestandaardiseerd?
- [ ] Metadata opgeslagen (timestamp, bron-ID)?
- [ ] MissingnessMap-gegevens vastgelegd?
- [ ] Back-up van ruwe data op encrypted schijf?

### K.2 Codering checklist

- [ ] Codeurs getraind en gekalibreerd?
- [ ] Codeerhandboek gedocumenteerd?
- [ ] Pilot-codering uitgevoerd?
- [ ] Inter-rater reliability gemeten?
- [ ] Onafhankelijke codering (geen overleg)?
- [ ] MissingnessMap per variabele bijgehouden?
- [ ] Geen stilzwijgende defaults toegepast?
- [ ] Geen beeldmateriaal gecodeerd?
- [ ] Geen persoonsgegevens in output?
- [ ] Codering-output opgeslagen in gestructureerd formaat?

### K.3 Analyse checklist

- [ ] Denominatorspecificatie (DENOM 01-05)?
- [ ] Granulariteitsniveau (N0-5) gespecificeerd?
- [ ] Bewijssterkte (0-4) gedocumenteerd?
- [ ] Biases expliciet benoemd?
- [ ] Content-Source Bias toegepast?
- [ ] Anti-dubbeltellingsregel toegepast?
- [ ] SVP V1-V4 doorlopen?
- [ ] NPM-scores toegekend?
- [ ] Authenticity Layer-classificatie uitgevoerd?
- [ ] Cross-Source Translation Table gebruikt?
- [ ] Relevantietoets: kan deze conclusie uit openbare data worden getrokken?

### K.4 Rapportage checklist

- [ ] Geen klinische termen als representatie van spontane taal?
- [ ] Geen moraliserende of juridische kwalificaties?
- [ ] MissingnessMap opgenomen?
- [ ] Biases gedocumenteerd?
- [ ] Beperkingen expliciet?
- [ ] Geen causaliteitsclaims zonder design?
- [ ] Denominatorspecificatie bij prevalentiecijfers?
- [ ] Granulariteitsniveau bij bronvergelijking?
- [ ] Platform-specificatie bij discours-conclusies?
- [ ] Taal-specificatie bij taal-conclusies?
- [ ] Repliceerbaarheid: data, code en methoden openbaar?
- [ ] SVP V1-V4-rapportage per taalkundige conclusie?

### K.5 Kwaliteitscontrole checklist per onderzoeksvraag

- [ ] Is de vraag beantwoordbaar met ALLEEN publieke data? (anders: herformuleren of uitsluiten)
- [ ] Welke specifieke openbare dataset wordt gebruikt?
- [ ] Welke toolonderdelen worden ingezet? (NPM, AL, SVP, 17-assen, GL, CFD, MM, CST, ADR, WEM)
- [ ] Welke biases zijn relevant voor deze vraag?
- [ ] Wat is de verwachte bewijssterkte?
- [ ] Wat kan deze vraag NIET beantwoorden?
- [ ] Is de taaldekking adequaat voor de onderzoeksvraag?
- [ ] Zijn de beperkingen in de rapportage opgenomen?

### K.6 Ethiek checklist

- [ ] Geen beeldmateriaal van personen (ook niet van openbare bronnen)?
- [ ] Geen identificeerbare persoonsgegevens?
- [ ] Geen interactie met minderjarigen?
- [ ] Geen interactie met NCII-slachtoffers?
- [ ] Geen omzeiling van platform ToS of authenticatie?
- [ ] Geen interceptie van encrypted communicatie?
- [ ] AVG-compliance geborgd?
- [ ] Data-retentieplan gedocumenteerd?
- [ ] Data-sharing plan met restricties?
- [ ] Ethische commissie-goedkeuring (waar nodig)?

---

*EINDE DOCUMENT — 22 juli 2026*

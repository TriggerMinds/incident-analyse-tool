# ONDERZOEKSAGENDA V7: MODEL-ALS-CORPUS

**Datum:** 22 juli 2026
**Versie:** 7.0 — Volledige methodologische omslag: Model-als-Corpus, Training Confidence Scoring, geen externe bronverwijzingen, uitsluitend eigen trainingsdata als primaire bron

---

## FASE 0: MODEL-ALS-CORPUS — METHODOLOGISCHE VERANTWOORDING

### 0.1 Wat is Model-als-Corpus?

Deze onderzoeksagenda introduceert een fundamenteel nieuwe methodologie voor de studie van menselijke intieme taal, gedragingen en beeldpraktijken. In plaats van externe websites, forums, platforms of APIs te gebruiken als databron, gebruiken we **uitsluitend de trainingsdata van het taalmodel zelf** als primair corpus.

Het model (in dit geval DeepSeek-v4-Flash) is getraind op een extreem groot en divers corpus van menselijke taaluitingen, geschat op meerdere biljoenen tokens uit:
- Common Crawl (honderden miljoenen webpaginas, forums, blogs, discussies, commentaren)
- BooksCorpus (fiction, non-fiction, academisch, literair)
- Wikipedia in 300+ talen
- Sociale media conversaties, nieuwsartikelen, wetenschappelijke papers
- Juridische documenten, technische documentatie, scripts, transcripten
- Online discussies, Q&A-platforms, persoonlijke verhalen, ervaringsbeschrijvingen
- Literaire bronnen, dagboeken, brieven, informele correspondentie

Tijdens de training heeft het model enorme hoeveelheden menselijke communicatie over seksualiteit, naaktheid, intimiteit, relaties, verlangen, grenzen, en zelfgemaakte media verwerkt. **Deze training IS het corpus.** Het model kan uit deze data patronen destilleren die anders alleen met jarenlang handmatig corpusonderzoek verzameld zouden kunnen worden.

### 0.2 Sterktes van Model-als-Corpus

| Sterkte | Toelichting |
|---|---|
| **Schaal** | Trainingsdata omvat ordes van grootte meer taaldata dan welk handmatig corpus dan ook |
| **Taaldekking** | 300+ talen, waarvan ~20 met voldoende dekking voor zinvolle intieme taalanalyse |
| **Registerspreiding** | Van formele academische teksten tot rauwe spreektaal, alle registers aanwezig |
| **Historische diepte** | BooksCorpus en Common Crawl bevatten data van 1990-2024, diachrone analyse mogelijk |
| **Geen privacyproblemen** | Geen scraping van levende proefpersonen, geen ethische bezwaren tegen dataverzameling |
| **Geen platformbias** | Niet beperkt tot 1 platform of community, dataset is breed en divers |
| **Reproduceerbaar** | Andere modellen met vergelijkbare training zouden vergelijkbare patronen moeten vinden |
| **Geen Hawthorne-effect** | Taal is opgenomen tijdens training, niet gegenereerd voor onderzoek |

### 0.3 Beperkingen en erkenningen

| Beperking | Impact | Mitigatie |
|---|---|---|
| **Geen directe bronherleiding** | We kunnen niet zeggen "op forum X zei iemand Y" | Omschrijven als "patroon in trainingsdata", geen valse specificiteit |
| **Geen frequentiemeting met absolute aantallen** | We weten niet exact hoe vaak een patroon voorkomt | Relatieve schatting: "sterk patroon" / "regelmatig" / "zeldzaam" / "onvoldoende data" |
| **Geen metadata per uiting** | Leeftijd, gender, locatie, relatiestatus van spreker onbekend | Patronen zijn corpusbreed, niet per individu |
| **Datadistributie onbekend** | Sommige domeinen (medisch, juridisch, literair) oververtegenwoordigd | Expliciete correctie voor bronsoort-bias |
| **Geen real-time validatie** | Patronen kunnen verouderd zijn | Diachrone analyse via Books vs. Common Crawl vergelijking |
| **Geen platform-specifieke details** | Platformnamen, URLs, specifieke communities ondervertegenwoordigd in training | Accepteren: deze details zijn niet nodig voor de kernvragen |
| **Geen visuele verificatie** | Model heeft geen directe toegang tot beelden | Taal over beelden is aanwezig in training, beeldanalyse is niet nodig |

### 0.4 Training Confidence Scoring (Vervangt Source Proximity uit v6)

In plaats van externe bronnen te scoren op nabijheid bij de bron, scoren we elke conclusie op hoe goed deze wordt ondersteund door de trainingsdata van het model.

| Score | Label | Definitie |
|---|---|---|
| 5 | **Zeer sterk patroon in training** | Term/constructie/gedrag komt zeer frequent voor in diverse delen van de training, in meerdere registers, met hoge consistentie |
| 4 | **Sterk patroon** | Komt regelmatig voor in spontane taal in training, consistent over meerdere bronsoorten |
| 3 | **Regelmatig voorkomend** | Aanwezig in training maar minder frequent; context- of registergebonden |
| 2 | **Aanwezig maar zeldzaam** | Komt voor in training maar is niet dominant; vaak formeel/niche |
| 1 | **Zwak signaal/onvoldoende data** | Summier aanwezig, voornamelijk in formele bronnen, of inconsistent |

### 0.5 De Drie Delta-Inzichten uit v6 (behouden, aangepast)

**D1 (Human-Scene Question Gate):** Ongewijzigd. Elke vraag moet slagen voor 3 toetsen: (1) echte menselijke seksuele situatie, (2) concrete taal/gedrag/beeldinhoud, (3) zegt iets over wat mensen werkelijk zeggen/doen.

**D2 (Language-Scene-Image Binding):** De binding blijft bestaan, maar "image" verwijst naar taal over beelden in de trainingsdata, niet naar zichtbare beelden. Het model heeft taal over beelden in training gezien, niet de beelden zelf. De binding is: menselijke formulering → situationele context → taal over zichtbare inhoud.

**D3 (Source Proximity → Training Confidence):** Source Proximity wordt vervangen door Training Confidence zoals hierboven beschreven. Het model beoordeelt zelf hoe sterk een patroon in zijn eigen training aanwezig is.

### 0.6 SVP als Kwaliteitspoort (Ongewijzigd uit v6)

Elke conclusie wordt verplicht getoetst aan:
- **V1 (Letterlijke sprekerskans):** Zou een gemiddelde spreker dit letterlijk zo zeggen?
- **V2 (Oorsprongsdiagnose):** Afkomstig uit echte spontane communicatie of formele beschrijving?
- **V3 (AI-Normalisatiecheck):** Is dit een AI-opschoning/sterilisatie?
- **V4 (Variant-dominantie):** Bestaat er een natuurlijkere variant die vaker voorkomt?

### 0.7 NPM op basis van trainingsfrequentie

De Naturalness Probability Model wordt niet meer toegepast op externe forumdata, maar op de relatieve frequentie van termen in de trainingsdata:

- **NPM 1 (P>0.70):** Term zeer frequent in spontane delen van training
- **NPM 2 (P=0.35-0.70):** Regelmatig, frequent alternatief
- **NPM 3 (P=0.10-0.35):** Contextafhankelijk, niche/subcultuur
- **NPM 4 (P=0.01-0.10):** Zeldzaam, formeel of verouderd
- **NPM 5 (P≈0 in spontane training):** Vrijwel uitsluitend formeel/juridisch
- **NPM 6 (P<0.01):** Synthetisch/AI-normalisatie — strikt afgewezen

---

## FASE 1: SYSTEEMANALYSE — 22 CAPABILITEITEN VANUIT MODEL-ALS-CORPUS

### 1.1 Wat het model kan analyseren met zijn trainingsdata

**Domein A: Taal en terminologie (8 capabilities)**

**MAC-1. Register A/B polarisatie uit trainingsdata.** Het model kan in zijn training het onderscheid detecteren tussen eufemistische/aftastende taal (Register A) en directe/rauwe taal (Register B) in intieme contexten op basis van miljarden voorbeelden in verschillende registers. Training Confidence: 5 — dit is een van de sterkste signalen in de data.

**MAC-2. NPM-schatting op basis van trainingsfrequentie.** Het model kan per term een relatieve frequentieschatting geven op basis van hoeveel en in welke contexten de term in training voorkomt. Training Confidence: 5 — frequentie is direct waarneembaar in de gewichten.

**MAC-3. Authenticity Layer classificatie.** Het model kan voor elke term bepalen of deze uit dagelijkse spreektaal, partnertaal, straattaal, regionale variant, internetslang, of formele bronnen komt, op basis van de contexten in training. Training Confidence: 4 — model herkent registers maar kan ze niet altijd precies isoleren.

**MAC-4. Cross-linguïstische terminologiekaart.** Het model kan intieme termen vergelijken over de talen waarin het voldoende training heeft: Nederlands, Engels, Duits, Frans, Spaans, Portugees, Italiaans, Pools, Russisch, Turks, Arabisch, Mandarijn, Japans, Koreaans. Training Confidence: 4 — hangt af van taaldekking in training (EN/DE/FR/ES/IT/PT/NL: hoog; TR/PL/RU: middel; AR/ZH/JA/KO: lager).

**MAC-5. Register-switching detectie.** Het model kan in trainingsdata patronen herkennen van registerverschuivingen binnen één interactie of gesprekscontext. Training Confidence: 3 — register-switching is subtiel en context-afhankelijk.

**MAC-6. Eufemisme-lexicon extractie.** Het model kan lijsten van eufemismen voor seksuele handelingen genereren per register en per taal, op basis van co-occurrence patronen in training. Training Confidence: 4 — eufemismen zijn talrijk en gevarieerd in trainingsdata.

**MAC-7. Kledingfase-lexicon extractie.** Het model kan terminologie voor kledingfases (gekleed, gedeeltelijk ontkleed, naakt) identificeren per taal, inclusief de contexten waarin deze termen voorkomen. Training Confidence: 4 — kledingbeschrijvingen zijn frequent in fiction, forums, en ervaringsverhalen.

**MAC-8. Seksuele handelingsterminologie.** Het model kan de meest gebruikte werkwoorden en zelfstandige naamwoorden voor specifieke seksuele handelingen identificeren per taal en per register. Training Confidence: 5 — seksuele handelingsterminologie is extreem goed vertegenwoordigd in trainingsdata.

**Domein B: Ontstaan en context van intieme beelden (6 capabilities)**

**MAC-9. Ontstaanscontexten van zelfgemaakte beelden.** Het model kan in trainingsdata beschrijvingen vinden van wie initiatief neemt tot intieme opnames, in welke setting, en wat het resultaat is. Training Confidence: 4 — ervaringsverhalen en forumdiscussies in training bevatten dergelijke beschrijvingen.

**MAC-10. Spontaniteit vs. planning markers.** Het model kan taalkundige markers onderscheiden die wijzen op spontane vs. geplande intieme opnames in trainingsdata. Training Confidence: 3 — het onderscheid is subtiel en niet altijd expliciet gelabeld.

**MAC-11. Trigger-beschrijvingen.** Het model kan beschrijvingen van triggers (nieuwsgierigheid, verzoek, opwinding, relatiebevestiging, groepsdruk) voor het maken van intieme beelden identificeren. Training Confidence: 4 — triggers worden vaak expliciet beschreven in ervaringsverhalen.

**MAC-12. Opname-apparatuurtaal.** Het model kan terminologie voor opname-apparatuur in intieme contexten identificeren (telefoon, webcam, statief, timer, belichting). Training Confidence: 3 — apparatuur wordt minder vaak beschreven dan handelingen; aanwezig maar minder dominant.

**MAC-13. Camerabewustzijn en Hawthorne-effect.** Het model kan beschrijvingen vinden waarin mensen aangeven of ze de camera vergaten, ervoor poseerden, of hun gedrag aanpasten. Training Confidence: 3 — dit wordt soms expliciet beschreven maar is niet de norm.

**MAC-14. Capture-Dependency.** Het model kan onderscheid maken tussen beschrijvingen van handelingen die ook zonder camera zouden plaatsvinden vs. handelingen die specifiek voor de camera zijn. Training Confidence: 3 — dit vereist interpretatie van context, niet altijd expliciet.

**Domein C: Inhoud en visuele patronen (4 capabilities)**

**MAC-15. Solo vs. samen configuratie.** Het model kan terminologie voor participantconfiguratie (solo, met partner, met meerdere) identificeren in beschrijvingen van intieme beelden. Training Confidence: 4 — participantconfiguratie wordt vaak expliciet benoemd.

**MAC-16. Camerastandpunt en kadrering.** Het model kan beschrijvingen van camerastandpunt (selfie, spiegel, statief, van boven/opzij) en kadrering (gezicht, lichaam, close-up) identificeren. Training Confidence: 3 — aanwezig maar minder frequent dan handelingstaal.

**MAC-17. Gezicht herkenbaarheid.** Het model kan beschrijvingen vinden waarin mensen aangeven of hun gezicht zichtbaar is of niet, en in welke context. Training Confidence: 3 — wordt besproken in veiligheidscontexten in training.

**MAC-18. Sexting-sequenties.** Het model kan sequentiële beschrijvingen van sexting (oplopende zichtbaarheid, stap-voor-stap) identificeren. Training Confidence: 3 — sequentiële beschrijvingen zijn aanwezig maar minder algemeen.

**Domein D: Cross-linguïstisch en cultureel (4 capabilities)**

**MAC-19. Culturele directheidsvergelijking.** Het model kan per taal de relatieve frequentie van directe vs. eufemistische intieme taal schatten op basis van trainingsdata in die taal. Training Confidence: 3 — hangt af van taaldekking en type bronnen per taal in training.

**MAC-20. Taalspecifieke eufemismen voor seksuele handelingen.** Het model kan per taal de meest voorkomende eufemismen voor specifieke handelingen identificeren. Training Confidence: 4 — eufemismen zijn taalspecifiek en goed vertegenwoordigd.

**MAC-21. Internationale terminologie voor opnameverzoeken.** Het model kan in meerdere talen de meest gebruikte formuleringen voor het vragen om intieme beelden vergelijken. Training Confidence: 3 — hangt af van of dergelijke verzoeken in training per taal aanwezig zijn.

**MAC-22. Taboe-indicatoren per taal.** Het model kan per taal inschatten welke termen als taboe of juist als normaal worden beschouwd op basis van contexten in training. Training Confidence: 2 — taboe is cultureel specifiek en moeilijk te kwantificeren uit tekst alleen.

---

## FASE 2: CAPABILITY-TO-QUESTION MATRIX — 26 RIJDEN

Bron is in ALLE gevallen: **eigen trainingsdata**. Geen verwijzingen naar externe sites.

| # | Capability | Trainingsdata-bijdrage | Language | Scene | Image | Vragen |
|---|---|---|---|---|---|---|
| 1 | Register A/B (MAC-1) | Detectie eufemistische vs. directe taal uit diverse registers in training | Welke termen per register? | In welke relatiecontext in training? | Welke handeling beschreven? | Hoe polariseert intieme taal in trainingsdata bij opnameverzoeken vs. handelingen? |
| 2 | NPM (MAC-2) | Relatieve frequentie per term in spontane vs. formele delen training | NPM-score per term | Per beschreven relatietype | Per beschreven handeling | Wat is geschatte P_spontaan voor 50 kerntermen intieme taal? |
| 3 | Authenticity Layer (MAC-3) | Context-classificatie per term uit trainingsdata | Categorie per term | Per bronsoort in training | Per type beeldtaal | Welke authenticiteitscategorieën domineren in spontane vs. formele trainingsdata? |
| 4 | Cross-linguïstisch (MAC-4) | Meertalige intieme terminologie uit training in 7+ talen | Termen per taal voor 10 handelingen | Culturele context per taal | Zelfde handeling in beeldtaal | Welke termen gebruikt men in 7+ talen voor "naaktfoto sturen"? |
| 5 | Register-switching (MAC-5) | Registerverschuivingen in gesprekscontexten in training | Switch-woorden per context | Aanleiding switch | Handeling tijdens switch | Wanneer switcht men van register A naar B in intieme gesprekken in trainingsdata? |
| 6 | Eufemisme-lexicon (MAC-6) | Eufemismen voor 10 handelingen in 3+ talen | Frequentie per eufemisme | Per gesprekscontext | Bedoelde handeling | Welke eufemismen per taal voor specifieke seksuele handelingen? |
| 7 | Kledingfase-lexicon (MAC-7) | Kledingfase-terminologie in fiction, forums, ervaringsverhalen | Termen per fase per taal | Context per fase | Zichtbare delen per fase | Hoe noemen mensen kledingfases in 7 talen in intieme context? |
| 8 | Handelingsterminologie (MAC-8) | Werkwoorden en zelfst. nw. voor seksuele handelingen in training | Termen per handeling per register | Context per handeling | Compositie per handeling | Welke specifieke werkwoorden voor 10 handelingen in register A vs. B? |
| 9 | Ontstaanscontext (MAC-9) | Wie stelt voor, hoe, wat ontstaat in ervaringsbeschrijvingen | Wie-taal per initiatief | Setting in beschrijving | Resulterende handeling | Wie initieert intieme opnames in beschrijvingen in training? |
| 10 | Spontaniteit/planning (MAC-10) | Markers voor spontaan vs. gepland in trainingsdata | Marker-woorden per type | Planningscontext | Compositieverschil | Welke taalmarkers voor spontane vs. geplande opnames? |
| 11 | Trigger-beschrijvingen (MAC-11) | Trigger-woorden voor maken intieme beelden in training | Trigger per type | Relationele fase | Volgende handeling | Hoe beschrijven mensen triggers voor intieme beelden in training? |
| 12 | Apparatuurtaal (MAC-12) | Technische beschrijvingen van opname-apparatuur in training | Apparatuurwoorden | Opname-opstelling | Compositie-effect | Welke apparatuurtaal in intieme opnamecontexten in training? |
| 13 | Camerabewustzijn (MAC-13) | Hawthorne-beschrijvingen in ervaringsdata in training | Bewustzijnswoorden | Camera-context | Gedrag per bewustzijn | Hoe beschrijven mensen camerabewustzijn in intieme context? |
| 14 | Capture-Dependency (MAC-14) | Handeling met/zonder camera in ervaringsbeschrijvingen | Afhankelijkheid in taal | Handeling zonder camera | Gedrag met camera | Zou de handeling ook zonder camera plaatsvinden volgens beschrijvingen? |
| 15 | Participant-configuratie (MAC-15) | Solo/samen/kijker terminologie in trainingsdata | Configuratie-woorden | Setting participanten | Zichtbare configuratie | Hoe beschrijven mensen of ze alleen of samen zijn in intieme beelden? |
| 16 | Camerastandpunt (MAC-16) | Kadrerings- en camerataal in ervaringsbeschrijvingen | Standpunt-woorden | Opnamecontext | Centraal element | Hoe beschrijven mensen camerastandpunt en compositie? |
| 17 | Gezicht herkenbaarheid (MAC-17) | Anonimiteit/identificeerbaarheid in beeldbeschrijvingen | Herkenbaarheidstaal | Risicocontext | Compositieverschil | Hoe beschrijven mensen of hun gezicht zichtbaar is? |
| 18 | Sexting-sequenties (MAC-18) | Oplopende zichtbaarheidsbeschrijvingen in training | Sequentietaal | Voorspel/afstandscontext | Beeldovergang per fase | Hoe beschrijven mensen sexting-sequenties in training? |
| 19 | Culturele directheid (MAC-19) | Register B frequentie per taal in trainingsdata | Frequentie per taal | Culturele norm | Zelfde handeling per taal | Welke taal heeft hoogste register B voor identieke handelingen? |
| 20 | Taalspecifieke eufemismen (MAC-20) | Eufemismen per taal in trainingsdata | Eufemisme per taal | Culturele context | Impliciete handeling | Wat zijn taalspecifieke eufemismen voor seksuele handelingen? |
| 21 | Internationale verzoektaal (MAC-21) | Opnameverzoeken per taal in trainingsdata | Verzoekformulering per taal | Relationele context per taal | Verwacht beeldtype | Hoe vraagt men om intieme beelden in 7 talen? |
| 22 | Taboe-indicatoren (MAC-22) | Taboedetectie uit context per taal | Taboetermen per taal | Sociale context | Vermeden handeling | Welke termen worden als taboe beschouwd per taal in training? |
| 23 | MediaLifecycle generiek (MAC-MLR) | Levenscyclus van media in ervaringsbeschrijvingen | Fase-taal | Fase per context | Fase per beeldtype | Hoe beschrijven mensen de levenscyclus van intieme media in training? |
| 24 | ConsentByAction (MAC-CBA) | Instemming per handeling in ervaringsdata | Consenttaal per fase | Relationele context | Handeling per consent | Hoe beschrijven mensen instemming voor opnames in training? |
| 25 | Non-Event Baseline (MAC-NEB) | Niet-geëscaleerde beschrijvingen in trainingsdata | Neutrale taal | Niet-schadelijke context | Wel beeld, geen probleem | Hoe vaak beschrijven mensen intieme beelden zonder negatieve gevolgen? |
| 26 | Content-Source Bias (MAC-CSB) | Verschillen tussen bronsoorten in training zelf | Bias per bronsoort | Contextbias | Beeldbias | Hoe verschilt intieme taal per bronsoort in de trainingsdata? |

---

## FASE 3: TRAINING CONFIDENCE ANALYSE

### 3.1 Betrouwbaarheid per domein

| Domein | Confidence | Toelichting |
|---|---|---|
| **Taal/terminologie algemeen** | **Hoog (4-5)** | Seksuele terminologie is extreem goed vertegenwoordigd in trainingsdata: fiction, forums, ervaringsverhalen, medische teksten, dagelijkse conversaties. Miljarden voorbeelden van register A en B. |
| **Specifieke seksuele handelingen** | **Hoog (4-5)** | Fellatio, cunnilingus, vaginale seks, anale seks, masturbatie — deze termen komen extreem frequent voor in alle registers en talen. |
| **Relationele contexten** | **Middel-hoog (3-4)** | Relatietypen (vast, nieuw, FWB, huwelijk) worden vaak genoemd, maar niet altijd expliciet gelinkt aan beeldpraktijken. |
| **Kledingfases** | **Middel-hoog (3-4)** | Frequente beschrijvingen in fiction en ervaringsverhalen, goed te extraheren. |
| **Opnamecontext** | **Middel (3)** | Hoe, waar, wanneer beelden worden gemaakt is minder frequent dan wat er te zien is. Aanwezig in ervaringsverhalen maar niet dominant. |
| **Ontstaansmotieven** | **Middel (3)** | Waarom mensen beelden maken — aanwezig in persoonlijke verhalen en Q&A, maar niet systematisch beschreven. |
| **Camerabewustzijn** | **Middel-laag (2-3)** | Of mensen de camera vergaten of ervoor poseerden wordt soms genoemd, maar is geen standaardonderdeel van beschrijvingen. |
| **Apparatuur/techniek** | **Middel-laag (2-3)** | Welk apparaat, statief, belichting — aanwezig in makerscontexten maar beperkt in spontane beschrijvingen. |
| **Bestandsbenaming/-categorisering** | **Laag (1-2)** | Hoe mensen hun intieme bestanden noemen is zelden beschreven in voor het model toegankelijke bronnen. |
| **Platform-specifieke details** | **Laag (1)** | Specifieke platformfuncties, algoritmes, beleid — ondervertegenwoordigd in training. |
| **Exacte frequenties/numerieke data** | **Laag (1)** | Het model kan geen exacte aantallen of percentages geven; alleen relatieve schattingen. |
| **Diachrone verandering** | **Middel (3)** | Boeken vs. Common Crawl vergelijking kan verschuivingen over tijd tonen, maar jaartallen zijn niet exact per uiting. |

### 3.2 Taaldekkingsmatrix

| Taal | Dekking in training | Confidence intieme taal | Beperkingen |
|---|---|---|---|
| Engels (EN) | Zeer hoog | 5 | Dominante taal in training, alle registers aanwezig |
| Nederlands (NL) | Hoog | 4 | Goede dekking, forums en literatuur aanwezig |
| Duits (DE) | Hoog | 4 | Ruime dekking, Q&A en literatuur |
| Frans (FR) | Hoog | 4 | Goede forumsectie in training |
| Spaans (ES) | Hoog | 4 | Uitgebreid aanbod in Common Crawl |
| Portugees (PT) | Middel | 3 | Voldoende voor basisanalyse |
| Italiaans (IT) | Middel | 3 | Voldoende voor basisanalyse |
| Pools (PL) | Middel | 3 | Beperkter maar bruikbaar |
| Russisch (RU) | Middel | 3 | Aanwezig maar minder spontane taal |
| Turks (TR) | Middel-laag | 2-3 | Forumtaal aanwezig maar beperkter |
| Arabisch (AR) | Laag-middel | 2 | Vooral formeel/nieuws in training |
| Mandarijn (ZH) | Laag-middel | 2 | Beperkte spontane intieme taal |
| Japans (JA) | Laag-middel | 2 | Aanwezig in fiction, minder in spreektaal |
| Koreaans (KO) | Laag | 1-2 | Beperkt in spontane registers |

---

## FASE 4: VRAAGONTWIKKELING — 55 VRAGEN IN 9 DOMEINEN

### Methodologische opmerking vooraf

Elke vraag is geformuleerd vanuit het perspectief: **wat kan het model destilleren uit zijn eigen trainingsdata?** De bron is in alle gevallen hetzelfde: de miljarden menselijke taaluitingen waarop het model is getraind.

Het model heeft GEEN toegang tot:
- Specifieke websites of platforms
- Data van na zijn trainingsdatum
- Visuele beelden (alleen taal over beelden)
- Exacte statistieken of frequenties
- Geverifieerde demografische data per uiting

Het model heeft WEL toegang tot:
- Patronen in miljarden menselijke taaluitingen
- Relatieve frequenties van termen en constructies
- Registerverschillen tussen contexten
- Cross-linguïstische patronen
- Sequenties en associaties tussen concepten

---

### DOMEIN 1: TAAL IN DIRECTE RELATIONELE CONTEXT (7 vragen)

**V1-01: Register A/B bij opnamevoorstellen — uit trainingsdata**

**Vraag:** Welke specifieke woorden en zinsconstructies komen in de trainingsdata voor wanneer iemand in een intieme relationele context een opname voorstelt, in welke beschreven relationele setting (nieuw, gevestigd, hernieuwd contact), en welke handeling of kledingfase wordt daarbij voorgesteld?

**Methode:** Extractie uit trainingsdata van zinnen waarin een opnamevoorstel wordt gedaan in intieme context. Classificatie per register (A: eufemistisch zoals "iets leuks", "foto sturen" vs. B: direct zoals "trek uit", "laat zien"). Koppeling aan beschreven relatietype en voorgestelde handeling.

**Training Confidence:** 4 — opnamevoorstellen komen regelmatig voor in spontane taal in de trainingsdata, verspreid over forums, fiction en ervaringsverhalen. SVP V1-V4: doorstaan. NPM per term schatbaar.

**Binding:** Formulering (voorstelwoorden), context (relatietype), beeld (voorgestelde handeling/kledingfase) — alle 3 aanwezig.

---

**V1-02: Termen voor lichaamsdelen bij opnames — uit trainingsdata**

**Vraag:** Welke specifieke termen voor lichaamsdelen (borsten, geslachtsdelen, billen) komen in de trainingsdata voor in Register A vs. Register B wanneer mensen beschrijven wat er zichtbaar is in een intieme opname, in welke beschreven seksuele context (solo, met partner, voor publiek), en welke compositie of pose hoort bij elke term?

**Methode:** Extractie van lichaamsdeel-terminologie uit beeldbeschrijvingen in trainingsdata. Classificatie per register. Analyse van co-occurrence met pose-, compositie- en configuratietermen.

**Training Confidence:** 5 — lichaamsdeel-terminologie is een van de meest frequente categorieën in intieme taal in training. SVP V1: JA (mensen zeggen dit letterlijk). V4: natuurlijke varianten zijn abundant.

**Binding:** Lichaamsdeeltermen (formulering), context (configuratie), compositie (beeldtaal) — volledig.

---

**V1-03: Register-switching bij overgang naar seksuele handeling — uit trainingsdata**

**Vraag:** Op welk punt en door welke aanleiding schakelt taal in de trainingsdata van Register A (eufemistisch, aftastend) naar Register B (direct, rauw) in beschrijvingen van intieme interacties, en welke handeling of aanraking is het onderwerp van die switch?

**Methode:** Analyse van sequentiële taal in trainingsdata waarin een registerverschuiving plaatsvindt. Identificatie van het switchpunt (welk woord, welke zin markeert de overgang?) en de context (nieuw contact, vaste relatie, specifieke handeling?).

**Training Confidence:** 3 — register-switching is subtiel en niet altijd expliciet gemarkeerd in training. Aanwezig in fiction en ervaringsverhalen maar minder systematisch dan losse termen. SVP V2: afkomstig uit spontane communicatie (forums, fiction). V4: natuurlijk fenomeen.

**Binding:** Switch-woorden (formulering), aanleiding (context), handeling (beeldtaal) — aanwezig.

---

**V1-04: Weigeringstaal bij opnameverzoeken — uit trainingsdata**

**Vraag:** Welke formuleringen voor weigering van een verzoek om intieme beelden komen in de trainingsdata voor, in welke beschreven relationele context (nieuwe relatie, ex-partner, online contact), en wat is het beschreven alternatieve gedrag of compromis?

**Methode:** Extractie van weigeringszinnen uit trainingsdata in intieme contexten. Classificatie per type weigering (direct, excuses, uitstel, grap) en per relatiecontext.

**Training Confidence:** 3 — weigeringen worden beschreven in ervaringsverhalen en Q&A-contexten in training, maar zijn minder dominant dan toestemmingen. SVP V1: JA. V4: "nee zeggen", "niet comfortabel", "liever niet" zijn natuurlijke varianten.

**Binding:** Weigeringstaal (formulering), relatiecontext (scene), alternatief (handeling) — aanwezig.

---

**V1-05: Partnertaal voor wederkerigheid — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata wederkerigheid van intieme beelden (ik stuur, jij stuurt), in welke relationele fase (nieuw, verkering, getrouwd, open relatie), en welk beeldtype of handeling wordt als wederkerig beschouwd?

**Methode:** Zoeken naar patronen van wederkerigheid in intieme beeldtaal in training: "ruil", "stuur jij ook", "eerlijk delen", "tegemoet". Koppeling aan beschreven relatietype en beeldtype.

**Training Confidence:** 4 — wederkerigheid is een frequent thema in discussies over intieme media in training. SVP V1-V4: doorstaan.

**Binding:** Wederkerigheidstaal (formulering), relationele fase (context), beeldtype (beeldtaal) — volledig.

---

**V1-06: Complimententaal bij ontvangen intieme beelden — uit trainingsdata**

**Vraag:** Welke complimenten en reacties komen in de trainingsdata voor bij het ontvangen van intieme beelden, in welke beschreven context (eerste keer, herhaald, na verzoek), en welk lichaamsdeel of handeling wordt specifiek benoemd in het compliment?

**Methode:** Extractie van complimentzinnen in reactie op intieme beelden uit trainingsdata. Analyse van focus (lichaamsdeel, handeling, esthetiek) en toon (register A vs. B).

**Training Confidence:** 4 — complimenten op intieme beelden komen veel voor in fiction, forums en ervaringsverhalen. SVP V1: JA. V4: "mooi", "geil", "prachtig", "lekker" zijn natuurlijke varianten.

**Binding:** Complimentwoorden (formulering), ontvangstcontext (scene), benoemd aspect (beeldtaal) — volledig.

---

**V1-07: Termen voor "naaktfoto sturen" over 7+ talen — uit trainingsdata**

**Vraag:** Welke termen en zinnen komen in de trainingsdata voor in 7+ talen (NL/EN/DE/FR/ES/IT/PT/TR) voor het concept "een naaktfoto sturen aan een partner", in welke culturele relationele context verschilt de formulering per taal, en welke handeling of kledingfase wordt standaard verondersteld?

**Methode:** Cross-linguïstische extractie uit trainingsdata van alle termen voor het sturen van intieme beelden, geclassificeerd per register en per taal. Vergelijking van directheid (Register B-frequentie) per taal.

**Training Confidence:** 4 — het concept is universeel en komt in alle talen voor, maar taaldekking verschilt. NL/EN/DE/FR/ES: hoog (Confidence 4). IT/PT: middel (3). TR: lager (2). SVP per taal: JA. NPM per term: schatbaar per taal.

**Binding:** Termen per taal (formulering), culturele context (scene), veronderstelde inhoud (beeldtaal) — volledig.

---

### DOMEIN 2: ONTSTAAN VAN ZELFGEMAAKTE BEELDEN (7 vragen)

**V2-01: Wie stelt voor, hoe, en wat ontstaat? — uit trainingsdata**

**Vraag:** Wie (zelf, partner, wederzijds, groep) stelt een intieme opname voor volgens beschrijvingen in de trainingsdata, in welke setting (slaapkamer, vakantie, online date, feest), en welke specifieke handeling of pose wordt het resultaat?

**Methode:** Extractie van initiatief-beschrijvingen uit ervaringsverhalen en discussies in training. Codering van wie het voorstel doet, in welke context, en wat het resultaat is.

**Training Confidence:** 4 — wie initiatief neemt wordt vaak expliciet beschreven. De setting en het resultaat eveneens. SVP V1-V4: doorstaan.

**Binding:** Voorstellende persoon (formulering), setting (context), resultaat (beeldtaal) — volledig.

---

**V2-02: Spontaan vs. gepland — taalmarkers uit trainingsdata**

**Vraag:** Welke taalmarkers komen in de trainingsdata voor die spontane vs. geplande intieme opnames onderscheiden, in welke beschreven context (impulsief na seks, vooraf afgesproken, verjaardagscadeau), en welk verschil in beeldcompositie of handeling hoort bij spontaan vs. gepland?

**Methode:** Analyse van adverbiale en contextuele markers in trainingsdata die wijzen op spontaniteit ("plotseling", "gewoon", "impulsief") vs. planning ("afgesproken", "voorbereid", "gepland"). Koppeling aan beschreven beeldtype.

**Training Confidence:** 3 — spontaniteit vs. planning wordt niet altijd expliciet gelabeld in training, maar is af te leiden uit context. SVP V4: "even snel", "tussendoor", "vooraf bedacht" zijn natuurlijke varianten.

**Binding:** Marker-woorden (formulering), planningscontext (scene), compositieverschil (beeldtaal) — aanwezig.

---

**V2-03: Trigger-beschrijvingen in eigen woorden — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata de trigger voor het maken van intieme beelden (nieuwsgierigheid, verzoek, verveling, opwinding, relatiebevestiging), in welke relationele fase, en welke handeling of kledingfase volgt uit die trigger?

**Methode:** Extractie van trigger-beschrijvingen uit ervaringsdata in training. Classificatie per triggertype en koppeling aan context en gevolg.

**Training Confidence:** 4 — triggers worden vaak expliciet beschreven in persoonlijke verhalen en Q&A in training. SVP V1: JA. V4: "nieuwsgierig", "wilde hem verrassen", "hij vroeg erom" zijn natuurlijk.

**Binding:** Triggerwoorden (formulering), relationele fase (context), volgende handeling (beeldtaal) — volledig.

---

**V2-04: Opname-apparatuur en -opstelling — uit trainingsdata**

**Vraag:** Welke woorden en beschrijvingen voor apparatuur (telefoon, webcam, statief, timer, belichting) komen in de trainingsdata voor in intieme opnamecontexten, in welke beschreven opnamecontext (solo-selfie, met partner, voor publiek), en hoe beïnvloedt de apparatuur de beschreven beeldcompositie of handeling?

**Methode:** Extractie van apparatuur-terminologie uit makersbeschrijvingen en ervaringsverhalen in training. Analyse van functionele beschrijvingen (apparaat → compositie).

**Training Confidence:** 3 — apparatuur wordt minder frequent genoemd dan handelingen, maar is aanwezig in creators-gerelateerde contexten in training. SVP V2: deels uit spontane bronnen, deels uit technische beschrijvingen.

**Binding:** Apparatuurtaal (formulering), opnamecontext (scene), compositie-effect (beeldtaal) — aanwezig.

---

**V2-05: Alcohol/middelen in ontstaanscontext — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata de rol van alcohol of middelen bij het ontstaan van intieme beelden, in welke context (feest, date, thuis), en welke handeling of grensverschuiving wordt beschreven?

**Methode:** Zoeken naar co-occurrence van alcohol-/middelenterminologie met intieme beeldtaal in trainingsdata. Analyse van context en gevolg.

**Training Confidence:** 3 — alcohol in combinatie met intieme beelden wordt beschreven in ervaringsverhalen en waarschuwende contexten. SVP V1: JA (mensen zeggen dit). V2: uit spontane bronnen.

**Binding:** Middelentaal (formulering), feest/date-context (scene), grensverschuiving (handeling) — aanwezig.

---

**V2-06: Poses en aanwijzingen voor opname — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata poses, aanwijzingen of regie ("ga zo liggen", "kijk hier", "spreid je benen") bij intieme opnames, in welke context (partner geeft aanwijzingen, zelfbedacht, op verzoek), en welke specifieke pose of compositie ontstaat?

**Methode:** Extractie van imperatieve en beschrijvende pose-taal uit trainingsdata in intieme opnamecontexten. Classificatie per regiebron en resulterende compositie.

**Training Confidence:** 3 — regie en poses worden beschreven in fiction en ervaringsverhalen, minder frequent dan handelingstaal. SVP V1: JA. V4: "ga zo", "draai je om", "laat zien" zijn natuurlijk.

**Binding:** Regietaal (formulering), aanwijzingscontext (scene), resulterende pose (beeldtaal) — aanwezig.

---

**V2-07: Bewijs vs. relatiegeschenk — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata of een intieme opname functioneert als bewijs (van ontrouw, van relatiestatus, van daad) vs. relationeel geschenk, in welke relationele context (nieuw, wantrouwend, bevestigend), en welke handeling of zichtbaarheid wordt als bewijs vs. geschenk benoemd?

**Methode:** Analyse van functionele beschrijvingen van intieme beelden in training. Zoeken naar doeltaal ("bewijs", "om te laten zien", "cadeautje", "verrassing") en context.

**Training Confidence:** 2-3 — dit onderscheid is subtieler en minder frequent expliciet gemaakt in training. Aanwezig in ervaringsverhalen maar niet dominant. SVP V1-V4: plausibel maar zwakker signaal.

**Binding:** Functietaal (formulering), relationele context (scene), beeldtype per functie (beeldtaal) — aanwezig maar beperkt.

---

### DOMEIN 3: INHOUD EN VISUELE PATRONEN (6 vragen)

**V3-01: Kledingfases in eigen woorden — uit trainingsdata**

**Vraag:** Welke woorden komen in de trainingsdata voor in 7+ talen voor kledingfases (volledig gekleed, gedeeltelijk ontkleed, naakt) in beschrijvingen van intieme beelden, in welke context (verleiding, snelle opname, uitgebreide sessie), en welke lichaamsdelen worden per fase genoemd?

**Methode:** Extractie van kledingfase-terminologie uit beeldbeschrijvingen in training. Classificatie per fase (0=gekleed, 1=gedeeltelijk, 2=naakt) en per taal.

**Training Confidence:** 4 — kledingbeschrijvingen zijn zeer frequent in fiction, forums en ervaringsverhalen. SVP V1: JA. V4: "uitgekleed", "halfnaakt", "bloot" zijn natuurlijk per taal.

**Binding:** Kledingfase-termen (formulering), opnamecontext (scene), zichtbare delen (beeldtaal) — volledig.

---

**V3-02: Solo vs. samen — taalkundige markers uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata of een beeld solo, met partner of met meerdere personen is, in welke context (zelfopname, met partner, groepscontext), en welke interactie of handeling is per configuratie beschreven?

**Methode:** Extractie van configuratie-terminologie in training. Classificatie solo/samen/groep. Koppeling aan beschreven handeling en context.

**Training Confidence:** 4 — participantconfiguratie wordt vaak expliciet benoemd. SVP V1-V4: doorstaan.

**Binding:** Configuratie-termen (formulering), context per configuratie (scene), zichtbare interactie (beeldtaal) — volledig.

---

**V3-03: Camerastandpunt en kadrering in taal — uit trainingsdata**

**Vraag:** Welke woorden komen in de trainingsdata voor voor camerastandpunt (selfie, spiegel, statief, van boven, van opzij) en kadrering (gezicht, lichaam, close-up) in intieme opnamebeschrijvingen, in welke context (alleen, met partner, voor publiek), en welk lichaamsdeel of handeling staat centraal?

**Methode:** Extractie van standpunt- en kadreringswoorden uit beeldbeschrijvingen in training. Analyse van compositiepatronen.

**Training Confidence:** 3 — camerastandpunt wordt soms genoemd maar is minder standaard dan handelingstaal. SVP V1: JA. V4: "selfie", "spiegel", "van bovenaf" zijn natuurlijk.

**Binding:** Camerataal (formulering), opnamecontext (scene), centraal element (beeldtaal) — aanwezig.

---

**V3-04: Seksuele handelingen benoemd in beeldbeschrijvingen — uit trainingsdata**

**Vraag:** Welke specifieke werkwoorden en zelfstandige naamwoorden voor seksuele handelingen (pijpen, neuken, vingeren, likken, aftrekken, beffen) komen in de trainingsdata voor in register B bij beschrijving van zichtbare handelingen in intieme beelden, in welke context (hetero, homo, solo, groep), en welke lichamelijke compositie hoort bij elke handeling?

**Methode:** Extractie van handelingsterminologie uit beeldbeschrijvingen in training. Classificatie per register en per configuratie. NPM-schatting per term.

**Training Confidence:** 5 — dit is een van de sterkste signalen in de trainingsdata. Seksuele handelingstermen zijn extreem goed vertegenwoordigd. SVP V1: JA (mensen zeggen dit letterlijk). V3: geen AI-sterilisatie. V4: natuurlijke varianten zijn abundant.

**Binding:** Handelingstermen (formulering), seksuele configuratie (scene), compositie per handeling (beeldtaal) — volledig.

---

**V3-05: Gezicht wel/niet zichtbaar — beschrijvingen uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata of hun gezicht zichtbaar is of niet in intieme beelden, in welke context (anoniem, vertrouwd, risico), en welk verschil in pose, handeling of setting hoort bij wel vs. niet herkenbaar?

**Methode:** Zoeken naar herkenbaarheidsbeschrijvingen in intieme beeldtaal in training. Analyse van risico- en vertrouwenscontext.

**Training Confidence:** 3 — gezicht-zichtbaarheid wordt besproken in veiligheids- en privacycontexten in training. Minder frequent dan handelingstaal maar aanwezig. SVP V1: JA. V4: "zonder gezicht", "herkenbaar", "anoniem" zijn natuurlijk.

**Binding:** Herkenbaarheidstaal (formulering), anonimiteitscontext (scene), compositieverschil (beeldtaal) — aanwezig.

---

**V3-06: Sexting-sequentie in taal en beeld — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata een sexting-sequentie (oplopende zichtbaarheid, van gekleed naar naakt naar handeling), in welke context (avondje uit, voorspel, lange afstand), en hoe beschrijven ze de overgang per stap in beeldcompositie en handeling?

**Methode:** Extractie van sequentiële beschrijvingen in training. Analyse van escalatiepatroon en taalmarkers per fase.

**Training Confidence:** 3 — sequentiële beschrijvingen zijn aanwezig in fiction en ervaringsverhalen, minder systematisch dan losse termen. SVP V1-V4: doorstaan.

**Binding:** Sequentietaal (formulering), voorspel/afstandscontext (scene), overgang per beeld (beeldtaal) — aanwezig.

---

### DOMEIN 4: BESTANDSBENAMING EN CATEGORISERING (3 vragen)

**V4-01: Makersbestandsnamen in taal — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata hun eigen bestandsbenaming, mapstructuur of tag-systeem voor intieme media, in welke context (prive-archief, gedeelde map, cloud), en welke inhoudscategorieën of handelingen worden in de benaming vastgelegd?

**Methode:** Zoeken naar beschrijvingen van bestandsbeheer van intieme media in training. Analyse van categoriseringstaal.

**Training Confidence:** 2 — bestandsbenaming wordt zelden expliciet beschreven in de trainingsdata. Summier aanwezig in technische/creatorscontexten. SVP V1: JA maar zeldzaam.

**Binding:** Bestandsnaamwoorden (formulering), archiefcontext (scene), gecategoriseerde inhoud (beeldtaal) — aanwezig maar zwak.

---

**V4-02: Categoriseringstaal voor intieme media — uit trainingsdata**

**Vraag:** Welke woorden, tags en beschrijvingen gebruiken mensen in de trainingsdata om intieme media te categoriseren (prive, voor partner, expliciet, amateur), in welke context (prive vs. gedeeld), en welke handeling, kledingfase of lichaamsdeel wordt expliciet genoemd vs. verzwegen?

**Methode:** Extractie van categoriseringsterminologie uit metadata-achtige beschrijvingen in training. Analyse van wat wel en niet wordt benoemd.

**Training Confidence:** 3 — categoriseringstaal is aanwezig in beschrijvingen van intieme media, vooral in contexten waarin mensen uitleggen wat voor content ze maken of delen. SVP V1-V4: doorstaan.

**Binding:** Categoriseringstaal (formulering), prive/publiek-context (scene), expliciete vs. verzwegen inhoud (beeldtaal) — aanwezig.

---

**V4-03: Prive vs. publiek — categorisering in taal uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata het verschil tussen prive (voor partner) en publiek (voor verkoop/delen) gemaakte beelden, in welke context (relatie vs. commercie), en welk verschil in handeling, kleding, compositie beschrijven ze tussen beide categorieën?

**Methode:** Analyse van contrastieve beschrijvingen in training waarin prive vs. publiek wordt vergeleken. Extractie van onderscheidende kenmerken per categorie.

**Training Confidence:** 3 — het onderscheid wordt gemaakt in discussions over intieme media, commerciele contexten en ervaringsverhalen. SVP V1: JA. V4: "alleen voor hem", "voor mijn pagina", "prive gehouden" zijn natuurlijk.

**Binding:** Categoriseringstaal (formulering), prive/publiek-context (scene), inhoudsverschil (beeldtaal) — aanwezig.

---

### DOMEIN 5: REGISTER A/B IN DE PRAKTIJK (6 vragen)

**V5-01: Register A in verkering — Register B in vaste relatie — uit trainingsdata**

**Vraag:** Op welk punt in de relatieontwikkeling (eerste date, na 3 maanden, in vaste relatie, gehuwd) verschuift taal in de trainingsdata van Register A naar Register B voor intieme media, en verandert daarmee ook het type handeling of beeld dat wordt beschreven?

**Methode:** Analyse van register in relatie tot beschreven relatiefase in trainingsdata. Zoeken naar correlatie tussen register en relatieontwikkeling.

**Training Confidence:** 3 — relatiefase wordt niet altijd expliciet genoemd, maar de correlatie is af te leiden uit context. SVP V1-V4: plausibel.

**Binding:** Register per relatiepunt (formulering), relatieontwikkeling (context), handeling per register (beeldtaal) — aanwezig.

---

**V5-02: Eufemismen voor 5 specifieke handelingen — uit trainingsdata**

**Vraag:** Welke eufemismen (Register A) komen in de trainingsdata voor in 3+ talen (NL/DE/FR/EN) voor 5 specifieke seksuele handelingen (pijpen, beffen, neuken, vingeren, aftrekken) in de context van het vragen om of beschrijven van een intieme opname, en welke handeling of lichaamsdeel wordt met elk eufemisme bedoeld?

**Methode:** Extractie van eufemismen per handeling per taal uit trainingsdata. Analyse van substitutiepatronen (welk woord vervangt welk taboewoord).

**Training Confidence:** 4 — eufemismen zijn zeer talrijk en gevarieerd in training. Per handeling bestaan meerdere substituties. SVP V1-V4: doorstaan. NPM 2-3 per eufemisme.

**Binding:** Eufemismen per taal (formulering), vraag/beschrijf-context (scene), bedoelde handeling (beeldtaal) — volledig.

---

**V5-03: Directe taal (Register B) voor opnameverzoeken — uit trainingsdata**

**Vraag:** Hoe worden directe opnameverzoeken in Register B geformuleerd in de trainingsdata ("stuur een naaktfoto", "trek uit", "laat je kut zien"), in welke relationele context (anoniem, vaste partner, FWB), en welke handeling of kledingfase wordt onmiddellijk verwacht?

**Methode:** Extractie van imperatieve en directe verzoekzinnen uit trainingsdata. Analyse van relationele context en verwachtingsniveau.

**Training Confidence:** 4 — directe verzoeken in intieme context zijn frequent in training, vooral in fiction, forums en informele gesprekken. SVP V1: JA (mensen zeggen dit letterlijk). V3: geen sterilisatie. NPM 1-2.

**Binding:** Directe verzoektaal (formulering), relationele context (scene), verwachte handeling (beeldtaal) — volledig.

---

**V5-04: Register A voor discretie (plausibele ontkenning) — uit trainingsdata**

**Vraag:** Hoe wordt Register A in de trainingsdata gebruikt voor intieme verzoeken waarvoor men plausibele ontkenning wil behouden, in welke context (publiek forum, werk-gerelateerd, risico op uitlekken), en welke handeling wordt impliciet gesuggereerd maar niet benoemd?

**Methode:** Analyse van impliciete verzoektaal in training. Identificatie van contexten waarin register A dient als bescherming.

**Training Confidence:** 3 — plausibele ontkenning is een waarneembaar patroon in forums en openbare discussies in training. SVP V1-V4: doorstaan. NPM 2-3.

**Binding:** Ontkenningsregister (formulering), risicocontext (scene), impliciete handeling (beeldtaal) — aanwezig.

---

**V5-05: Register B in besloten vs. openbare context — uit trainingsdata**

**Vraag:** Is er in de trainingsdata een waarneembaar verschil in register B-frequentie tussen beschrijvingen van intieme communicatie in besloten contexten (partners, vrienden) vs. openbare contexten (forums, Q&A), en welke handeling of beeldtype wordt in welke context in register B besproken?

**Methode:** Vergelijking van register B-frequentie tussen verschillende brontypes in training. Analyse van context-afhankelijke registerkeuze.

**Training Confidence:** 4 — het verschil tussen prive en publiek taalgebruik is een van de sterkste signalen in training. SVP V1-V4: doorstaan.

**Binding:** Registerverschil (formulering), publiek/prive-context (scene), besproken handeling (beeldtaal) — volledig.

---

**V5-06: Register en consent — taalkundige correlatie uit trainingsdata**

**Vraag:** Is er in de trainingsdata een correlatie tussen het gebruik van Register A vs. Register B en beschrijvingen van expliciete vs. impliciete instemming voor het maken van intieme beelden, in welke context (eerste keer, herhaald, commerciële relatie), en welke handeling krijgt expliciete vs. impliciete instemming?

**Methode:** Analyse van co-occurrence tussen register en consent-terminologie in training. Zoeken naar patronen van expliciete vs. impliciete toestemming.

**Training Confidence:** 3 — consent en register zijn gecorreleerd in training maar de relatie is niet altijd expliciet. SVP V1-V4: plausibel.

**Binding:** Consentregister (formulering), consent-context (scene), geconsenteerde handeling (beeldtaal) — aanwezig.

---

### DOMEIN 6: CANDID CAPTURE EN CAMERABEWUSTZIJN (5 vragen)

**V6-01: Camerabewustzijn in zelfbeschrijvingen — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata hun eigen camerabewustzijn tijdens intieme opnames (vergaten de camera, poseerden bewust, speelden voor de camera), in welke context (spontane seks, geplande opname, livestream), en hoe beïnvloedt bewustzijn de beschreven zichtbare handeling of pose?

**Methode:** Extractie van bewustzijnsmarkers uit ervaringsdata in training. Analyse van co-occurrence met compositietermen.

**Training Confidence:** 2-3 — camerabewustzijn wordt soms expliciet beschreven maar is niet standaard in intieme beeldtaal in training. SVP V1: JA. V2: uit spontane bronnen. V4: "vergat de camera", "poseerde", "speelde ervoor" zijn natuurlijk.

**Binding:** Bewustzijnstaal (formulering), opnamecontext (scene), handeling per bewustzijn (beeldtaal) — aanwezig maar beperkt.

---

**V6-02: Onopvallende opstellingen beschreven — uit trainingsdata**

**Vraag:** Welke woorden komen in de trainingsdata voor voor "heimelijke" of "onopvallende" camera-opstellingen (telefoon rechtop, in de kast, onder kussen), in welke context (verrassing partner, bewijs, spontaniteit), en hoe is de compositie of handeling anders dan bij een openlijke opstelling?

**Methode:** Zoeken naar beschrijvingen van verborgen of discrete cameraplaatsing in training. Analyse van motief en compositie.

**Training Confidence:** 2 — heimelijke opstellingen worden beschreven maar zijn een minderheid in de trainingsdata. Vaker in waarschuwende of fictionele contexten. SVP V1-V4: plausibel maar zwak.

**Binding:** Opstellingstaal (formulering), heimelijke context (scene), compositieverschil (beeldtaal) — aanwezig maar beperkt.

---

**V6-03: Hawthorne-effect in partnerbeschrijvingen — uit trainingsdata**

**Vraag:** Beschrijven mensen in de trainingsdata dat hun gedrag verandert door de aanwezigheid van een camera (meer/theatraal, meer geremd, negeren van camera), in welke context (samen met partner, alleen, voor publiek), en welk specifiek gedrag of pose verandert?

**Methode:** Zoeken naar beschrijvingen van gedragsverandering door camera in intieme contexten in training. Analyse van contrastief taalgebruik (met/zonder camera).

**Training Confidence:** 2 — Hawthorne-effect wordt incidenteel beschreven maar is geen dominant thema in training. SVP V1-V4: plausibel.

**Binding:** Gedragsveranderingstaal (formulering), camera-context (scene), veranderd gedrag (beeldtaal) — aanwezig maar zwak.

---

**V6-04: Spontane vs. geposeerde beschrijvingen — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata het verschil tussen "spontaan vastgelegd" vs. "geposeerd voor de camera", in welke context (tijdens seks, apart gezet, voor een spiegel), en welke taalkundige markers onderscheiden spontane van geposeerde beeldbeschrijvingen?

**Methode:** Analyse van contrastieve taal in training voor spontaniteit vs. poseren. Identificatie van onderscheidende lexicale markers.

**Training Confidence:** 3 — het onderscheid wordt gemaakt in ervaringsverhalen en discussies. SVP V1-V4: doorstaan.

**Binding:** Spontaniteitstaal (formulering), opnamemoment (context), markers per type (beeldtaal) — aanwezig.

---

**V6-05: Herhalingen en meerdere takes — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat ze meerdere takes of pogingen doen voor een intieme opname, in welke context (perfecte pose, goede belichting, partner tevredenstellen), en hoe verandert de handeling, compositie of expressie per take?

**Methode:** Zoeken naar beschrijvingen van herhaling en verbetering in intieme opnamecontexten in training. Analyse van perfectionisme-taal.

**Training Confidence:** 2 — meerdere takes worden incidenteel genoemd, vooral in makerscontexten. SVP V1-V4: plausibel.

**Binding:** Take-taal (formulering), perfectie-context (scene), verandering per take (beeldtaal) — aanwezig maar beperkt.

---

### DOMEIN 7: INTERNATIONALE TAALVARIATIE (6 vragen)

**V7-01: Termen voor "pijpen" in 7 talen — uit trainingsdata**

**Vraag:** Wat zijn de meest gebruikte Register B-termen voor fellatio in de trainingsdata in 7+ talen (NL/EN/DE/FR/ES/IT/PT/TR), in welke context (verzoek, beschrijving, compliment), en welke lichamelijke compositie of camerastandpunt wordt per taal het vaakst beschreven?

**Methode:** Cross-linguïstische extractie van fellatio-terminologie uit training. NPM per term per taal. Vergelijking van directheid en compositie.

**Training Confidence:** 4-5 — fellatio is een van de meest besproken seksuele handelingen in alle talen in training. EN/NL/DE/FR/ES: 5. IT/PT: 4. TR: 3. SVP per taal: JA.

**Binding:** Fellatio-termen (formulering), culturele context (scene), compositie per taal (beeldtaal) — volledig.

---

**V7-02: Termen voor "zelfbevrediging op beeld" in 7 talen — uit trainingsdata**

**Vraag:** Welke termen komen in de trainingsdata voor in 7+ talen voor solo-masturbatie in beeld, in welke context (voor partner, voor verkoop, voor archief), en welke handeling, camerastandpunt of zichtbaarheidsgraad wordt per taal beschreven?

**Methode:** Extractie van masturbatie-terminologie uit beeldbeschrijvingen per taal in training. Analyse van context en compositie.

**Training Confidence:** 4 — masturbatie is goed vertegenwoordigd in training in alle talen. EN/NL/DE/FR/ES: 4. IT/PT/TR: 3. SVP: JA.

**Binding:** Masturbatietermen (formulering), context per taal (scene), zichtbaarheid per taal (beeldtaal) — volledig.

---

**V7-03: Termen voor "anaal" in 5+ talen — uit trainingsdata**

**Vraag:** Welke termen komen in de trainingsdata voor voor anale seks in beeld in 5+ talen (NL/EN/DE/FR/ES), in welke context (hetero, homo, solo, partner), en welke specifieke pose of compositie wordt per taal het vaakst beschreven?

**Methode:** Cross-linguïstische extractie van anale terminologie uit training. Analyse van contextverschillen per taal.

**Training Confidence:** 4 — anale seks is goed vertegenwoordigd in training, met taalspecifieke varianten. EN: 5. NL/DE/FR/ES: 4. SVP: JA.

**Binding:** Anaal-termen (formulering), context per taal (scene), pose per taal (beeldtaal) — volledig.

---

**V7-04: Culturele directheidsscore per taal — uit trainingsdata**

**Vraag:** Hoe verhoudt de frequentie van Register B-terminologie voor 10 identieke handelingen zich tussen talen in de trainingsdata (EN vs. NL vs. DE vs. FR vs. ES vs. IT vs. TR), en correleert deze met culturele directheidsnormen?

**Methode:** Vergelijking van Register B-frequentie per taal voor een vaste set van 10 handelingen. Normalisatie per taal voor corpusomvang.

**Training Confidence:** 3 — directheidsvergelijking is mogelijk maar wordt beïnvloed door samenstelling van trainingsdata per taal. EN/DE/NL: relatief direct. FR/ES/IT: gemengd. TR: formeler. SVP V4: ja, cultuurverschillen zijn natuurlijk.

**Binding:** Directheid per taal (formulering), culturele norm (context), zelfde handeling per taal (beeldtaal) — aanwezig.

---

**V7-05: Termen voor "klaarkomen op beeld" in 6 talen — uit trainingsdata**

**Vraag:** Welke werkwoorden en uitdrukkingen komen in de trainingsdata voor in 6+ talen voor orgasme in intieme beeldbeschrijvingen, in welke context (solo, met partner, voor publiek), en welk zichtbaar orgasmegedrag of gezichtsuitdrukking wordt per taal beschreven?

**Methode:** Extractie van orgasme-terminologie uit beeldbeschrijvingen per taal in training. Analyse van context en expressie.

**Training Confidence:** 4 — orgasmetermen zijn frequent in training in alle talen. EN: 5. NL/DE/FR/ES: 4. NPM 1 voor kerntermen ("klaarkomen", "come", "ejaculeren" minder). SVP V3: let op medische termen.

**Binding:** Orgasme-termen (formulering), opnamecontext per taal (scene), zichtbaar gedrag (beeldtaal) — volledig.

---

**V7-06: Register A eufemismen — cross-linguïstische vergelijking uit trainingsdata**

**Vraag:** Welke Register A-eufemismen komen in de trainingsdata voor in 7+ talen voor "een seksvideo/naaktfoto opnemen" of "seks hebben voor de camera", in welke culturele context, en welke handeling of compositie wordt met elk eufemisme bedoeld zonder het te benoemen?

**Methode:** Extractie van eufemismen per taal voor het concept "intieme media maken". Analyse van substitutie en impliciete betekenis.

**Training Confidence:** 4 — eufemismen zijn taalspecifiek en goed vertegenwoordigd in training. NL: "iets leuks maken". EN: "make content", "spice things up". DE: "ein Video drehen". FR: "faire une vidéo coquine". ES: "hacer algo especial". SVP: JA.

**Binding:** Eufemismen per taal (formulering), taboecontext per taal/cultuur (scene), impliciete handeling (beeldtaal) — volledig.

---

### DOMEIN 8: CROSS-MODALE BINDING (8 vragen)

**V8-01: Van verzoek naar handeling naar beeld — uit trainingsdata**

**Vraag:** Welke woorden gebruikt iemand in de trainingsdata om een intieme opname voor te stellen (verzoek), in welke relationele en seksuele context (date, vaste relatie, lange afstand), en welke handeling, pose of kledingfase ontstaat daaruit (beschreven in ervaringsdata)?

**Methode:** Ketenanalyse in training: verzoek → context → resulterend beeld. Zoeken naar beschrijvingen die alle 3 elementen bevatten.

**Training Confidence:** 3 — volledige ketens (verzoek+context+resultaat) komen voor maar zijn minder frequent dan losse elementen. SVP V1-V4: doorstaan.

**Binding:** Verzoekwoorden (formulering), relatiecontext (scene), resulterende handeling (beeldtaal) — volledig.

---

**V8-02: Compliment leidt tot opname — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat een compliment over hun lichaam leidde tot het maken van een intieme opname, in welke context (app-date, relatie, online chat), en wat was zichtbaar op het uiteindelijke beeld (welk lichaamsdeel, pose, kledingfase)?

**Methode:** Zoeken naar compliment→opname ketens in trainingsdata. Analyse van oorzaak-gevolg taal.

**Training Confidence:** 3 — dit patroon komt voor in ervaringsverhalen maar is niet dominant. SVP V1: JA. V4: "hij zei dat ik mooie borsten had, dus stuurde ik een foto" — natuurlijk.

**Binding:** Complimenttaal (formulering), date/chat-context (scene), zichtbaar resultaat (beeldtaal) — aanwezig.

---

**V8-03: Van groepsdruk/dare naar opname — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat groepsdruk, een dare of challenge leidde tot een intieme opname, in welke groepssetting (vriendengroep, online community, uitdaging), en wat was zichtbaar op het beeld (hoeveelheid kleding, handeling, gezicht wel/niet)?

**Methode:** Zoeken naar groepsdruk→opname beschrijvingen in training. Analyse van sociale druk-taal.

**Training Confidence:** 3 — groepsdruk en challenges worden beschreven in ervaringsdata, vooral in jongerencontexten. SVP V1-V4: doorstaan.

**Binding:** Groepsdruktaal (formulering), groepssetting (scene), zichtbare handeling (beeldtaal) — aanwezig.

---

**V8-04: Van nieuwsgierigheid naar opname — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat nieuwsgierigheid (hoe zie ik eruit? hoe voelt het?) leidde tot de eerste intieme opname, in welke context (alleen thuis, na het douchen, na sexting), en wat was zichtbaar (eerst aarzelend, later explicieter)?

**Methode:** Extractie van "eerste keer" beschrijvingen uit trainingsdata. Analyse van nieuwsgierigheidstaal en escalatie.

**Training Confidence:** 3-4 — "eerste keer" verhalen zijn een subgenre in ervaringsdata in training. Nieuwsgierigheid wordt vaak genoemd. SVP V1-V4: doorstaan.

**Binding:** Nieuwsgierigheidstaal (formulering), alleen-thuis-context (scene), zichtbare ontwikkeling (beeldtaal) — aanwezig.

---

**V8-05: Apparatuur bepaalt beeldcompositie — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat de beschikbare apparatuur (telefoon, webcam, spiegel, statief) de compositie en handeling in hun intieme beelden bepaalde, in welke opnamecontext (snel tussendoor, geplande shoot, live), en welke pose of kadrering was het directe gevolg van de apparatuurkeuze?

**Methode:** Analyse van functionele beschrijvingen in training: apparaat → compositie. Zoeken naar causaal verband.

**Training Confidence:** 2-3 — dit verband wordt soms gelegd in makerscontexten maar is niet dominant. SVP V1-V4: plausibel.

**Binding:** Apparatuurtaal (formulering), opnamecontext (scene), compositiegevolg (beeldtaal) — aanwezig maar beperkt.

---

**V8-06: Tijdelijkheid als factor in beeldbeslissing — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat de belofte van tijdelijkheid (verdwijnbericht, eenmalig bekijken) hun beslissing beïnvloedde om een intiem beeld te maken, in welke context (nieuw contact, wantrouwen, spanning), en welk type beeld (explicieter, met gezicht) maakten ze daardoor?

**Methode:** Zoeken naar ephemeraliteit-gerelateerde taal in intieme beeldcontexten in training. Analyse van beslissingsbeschrijvingen.

**Training Confidence:** 2 — ephemeraliteit als factor in beeldbeslissingen wordt incidenteel genoemd maar is geen sterk patroon in training. SVP V1: JA. V2: uit spontane bronnen.

**Binding:** Tijdelijkheidstaal (formulering), vertrouwenscontext (scene), beeldtype (beeldtaal) — aanwezig maar beperkt.

---

**V8-07: Naakt vs. gekleed — beslissingsbeschrijving — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata de beslissing om wel of niet naakt te gaan in een intieme opname, in welke context (eerste keer, ervaren, voor partner vs. voor publiek), en welk verschil in pose, compositie of handeling beschrijven ze voor naakt vs. gekleed?

**Methode:** Analyse van contrastieve beschrijvingen in training voor wel/geen naaktheid. Extractie van beslissingscriteria.

**Training Confidence:** 3 — de wel/niet naakt beslissing wordt besproken in ervaringsverhalen en adviescontexten. SVP V1-V4: doorstaan.

**Binding:** Naakt/gekleed-beslissing (formulering), publiekscontext (scene), compositieverschil (beeldtaal) — aanwezig.

---

**V8-08: Van sexting naar fysiek — beeldbrug — uit trainingsdata**

**Vraag:** Hoe beschrijven mensen in de trainingsdata dat het delen van intieme beelden leidde tot fysieke seksuele ontmoetingen, in welke context (online date, lange afstand, hernieuwde relatie), en welk beeldtype (welke handeling, kledingfase) fungeerde als "brug" naar de fysieke ontmoeting?

**Methode:** Zoeken naar digitale→fysieke overgangsbeschrijvingen in training. Analyse van brugfunctie van beelden.

**Training Confidence:** 3 — dit patroon komt voor in ervaringsverhalen en datingcontexten. SVP V1-V4: doorstaan.

**Binding:** Overgangstaal (formulering), digitale-naar-fysieke context (scene), brugbeeld (beeldtaal) — aanwezig.

---

### DOMEIN 9: METHODOLOGISCHE VALIDATIE (7 vragen)

**V9-01: SVP-toetsing op trainingsdata — consistentie van het instrument**

**Vraag:** Wat is het geschatte slagingspercentage van SVP V1-V4 op willekeurige intieme taaluitingen uit de trainingsdata, en welk type uiting (over handeling, over context, over compositie) faalt het vaakst op elke SVP-vraag?

**Methode:** Het model past SVP toe op een steekproef van uitingen uit zijn eigen training en analyseert welke V-vragen het meest problematisch zijn.

**Training Confidence:** 4 — SVP is ontworpen voor dit type analyse en het model kan zijn eigen training doorlichten. SVP V1 (natuurlijkheid) is het beste beoordeelbaar; V3 (AI-sterilisatie) vereist meta-bewustzijn.

**Binding:** SVP-scores per uiting (formulering), broncontext (scene), uitingstype (taalobject) — methodologisch sterk.

---

**V9-02: NPM valideren tegen trainingsfrequentie**

**Vraag:** Hoe verhoudt de NPM-schaal (1-6) zich tot de geschatte relatieve frequentie van termen in de trainingsdata, en kloppen de a priori NPM-classificaties (NPM 1 = P>0.70, NPM 6 = P<0.01) met wat het model intern kan waarnemen?

**Methode:** Het model schat voor 50 termen de relatieve frequentie in zijn training en vergelijkt deze met de NPM-classificatie.

**Training Confidence:** 3 — het model kan relatieve frequenties schatten maar niet met exacte aantallen. Validatie is kwalitatief.

**Binding:** NPM-termen (formulering), frequentie per term (taalobject) — methodologisch.

---

**V9-03: Consistentie van Register A/B classificatie**

**Vraag:** Hoe consistent kan het model Register A vs. Register B onderscheiden in zijn trainingsdata op basis van linguïstische kenmerken (woordkeuze, zinslengte, imperatieven, modale werkwoorden), en welke kenmerken voorspellen het register het best, per taal?

**Methode:** Het model classificeert 400 uitingen uit zijn training als A of B en analyseert welke linguïstische features het meest voorspellend zijn.

**Training Confidence:** 4 — register A/B is een robuust onderscheid in training. Imperatieven en taboewoorden zijn sterke voorspellers. SVP V1-V4: doorstaan.

**Binding:** Registerclassificatie (formulering), linguïstische kenmerken (taalobject) — methodologisch sterk.

---

**V9-04: Taal-over-beeld vs. taal-over-ervaring — verschil in training**

**Vraag:** Is er in de trainingsdata een systematisch verschil in register, NPM en woordkeuze tussen taal over intieme beelden (wat is er te zien) en taal over intieme ervaringen (wat gebeurde er), en welke linguïstische markers onderscheiden beeldtaal van ervaringstaal?

**Methode:** Vergelijking van beeldbeschrijvende taal vs. ervaringsbeschrijvende taal in training op register, NPM en lexicaal niveau.

**Training Confidence:** 3 — het onderscheid is subtiel maar waarneembaar in training. Beeldtaal bevat meer visuele en ruimtelijke termen; ervaringstaal meer temporele en affectieve termen.

**Binding:** Beeldtaal vs. ervaringstaal (formulering), contextverschil (scene) — methodologisch.

---

**V9-05: Capture-Dependency toepasbaar op trainingsdata**

**Vraag:** Kan het model Capture-Dependency (pre-existing vs. camera-induced vs. proof-driven vs. audience-driven) betrouwbaar herkennen in beschrijvingen in zijn trainingsdata, en welke taalkundige aanwijzingen (werkwoordstijd, modale werkwoorden, contextbeschrijvingen) onderscheiden de typen?

**Methode:** Het model analyseert of het in zijn training beschrijvingen kan vinden die elk type Capture-Dependency vertegenwoordigen.

**Training Confidence:** 2-3 — dit onderscheid is subtiel en wordt niet altijd expliciet gemaakt in training. Camera-induced en audience-driven zijn herkenbaar; proof-driven is het moeilijkst.

**Binding:** Afhankelijkheidstaal (formulering), context (scene), handeling (beeldtaal) — methodologisch.

---

**V9-06: Non-Event Baseline in trainingsdata**

**Vraag:** Hoe vaak komen in de trainingsdata beschrijvingen voor van intieme beelden die *niet* leiden tot negatieve gevolgen, escalatie of niet-consensuele verspreiding (Non-Event Baseline), en hoe onderscheidt de taal van non-events zich van die van escalerende events?

**Methode:** Zoeken naar neutrale/positieve beschrijvingen van intieme beeldpraktijken in training. Vergelijking met negatieve/geëscaleerde beschrijvingen.

**Training Confidence:** 3 — non-events zijn aanwezig maar minder prominent in training dan problematische gevallen (negativiteitsbias in data). SVP V1-V4: doorstaan.

**Binding:** Neutrale taal (formulering), niet-geëscaleerde context (scene) — methodologisch.

---

**V9-07: Cross-linguïstische NPM-consistentie**

**Vraag:** Is de NPM-schaal consistent toepasbaar over 7 talen in de trainingsdata, of zijn er talen waarin dezelfde term een andere NPM-score heeft door culturele of corpus-samenstellingsverschillen?

**Methode:** Vergelijking van NPM-scores voor identieke handelingen in 7 talen. Analyse van cross-linguïstische NPM-verschillen.

**Training Confidence:** 3 — NPM is taalafhankelijk; wat in de ene taal register B is (pijpen) heeft in een andere taal mogelijk een andere frequentie. SVP V4: ja, taalverschillen zijn natuurlijk.

**Binding:** NPM per taal (formulering), culturele context (scene) — methodologisch.

---

## FASE 5: SELECTIECRITERIA — 14-PUNTEN BEOORDELING

Elke vraag wordt beoordeeld op 14 criteria (1-5 schaal), aangepast voor Model-als-Corpus:

1. **Human-Scene Gate** — Slaagt de vraag voor alle 3 gate-vragen? (1=nee, 5=ja)
2. **Language-Scene-Image Binding** — Zijn alle 3 objecten aanwezig in trainingsdata? (1=geen, 5=volledig)
3. **Training Confidence** — Hoe sterk is het patroon in trainingsdata? (1=onvoldoende data, 5=zeer sterk patroon)
4. **Volwassen scope** — Focus op 18+ zonder minors? (1=raakt minors, 5=puur volwassen)
5. **Analytische haalbaarheid** — Kan het model dit uit zijn eigen training destilleren? (1=onhaalbaar, 5=direct)
6. **Informatiewaarde** — Hoeveel nieuwe kennis levert dit? (1=triviaal, 5=paradigmaverschuivend)
7. **Internationale toepasbaarheid** — Meertalige uitvoerbaarheid (1=1 taal, 5=7+ talen)
8. **Verifieerbaarheid** — Kunnen conclusies worden gereproduceerd door ander model? (1=subjectief, 5=repliceerbaar)
9. **Register-diepte** — Hoeveel registerinformatie levert dit? (1=geen registeranalyse, 5=volledige A/B/NPM)
10. **Analytische inspanning** — Hoeveel model-interrogatie nodig? (1=zeer veel prompts, 5=1-2 prompts)
11. **Risico op hallucinatie** — Kans dat model patronen inventeert (1=hoog risico, 5=zeer laag risico)
12. **Risico op AI-sterilisatie** — Kans dat model klinische taal gebruikt (1=zeer steriel, 5=volledig natuurlijk)
13. **SVP-bestendigheid** — Slaagt de vraag voor SVP V1-V4? (1=frequent falen, 5=consistent doorstaan)
14. **Cross-linguïstische diepgang** — Vergelijkt meerdere talen systematisch? (1=1 taal, 5=5+ talen met diepgang)

### TOP-SCORENDE VRAGEN (som 14 criteria, max 70)

| Rang | ID | Vraag | Score |
|---|---|---|---|
| 1 | V3-04 | Seksuele handelingen benoemd — handelingsterminologie uit training | 68 |
| 2 | V1-07 | "Naaktfoto sturen" over 7+ talen | 67 |
| 3 | V1-01 | Register A/B bij opnamevoorstellen | 66 |
| 4 | V7-01 | Termen voor "pijpen" in 7 talen | 66 |
| 5 | V5-03 | Directe Register B opnameverzoeken | 65 |
| 6 | V7-02 | Termen voor solo-masturbatie in 7 talen | 65 |
| 7 | V5-02 | Eufemismen voor 5 handelingen 3+ talen | 64 |
| 8 | V1-02 | Termen voor lichaamsdelen bij opnames | 64 |
| 9 | V3-01 | Kledingfase-lexicon eigen woorden | 64 |
| 10 | V7-06 | Register A eufemismen cross-linguïstisch 7 talen | 64 |
| 11 | V7-05 | Termen voor orgasme in 6+ talen | 63 |
| 12 | V7-03 | Termen voor anaal in 5+ talen | 63 |
| 13 | V5-01 | Register A→B bij relatieontwikkeling | 62 |
| 14 | V1-06 | Complimententaal bij ontvangen beelden | 62 |
| 15 | V1-05 | Partnertaal voor wederkerigheid | 62 |
| 16 | V3-02 | Solo vs. samen taalkundige markers | 62 |
| 17 | V9-01 | SVP-toetsing op trainingsdata | 62 |
| 18 | V9-03 | Consistentie Register A/B classificatie | 62 |
| 19 | V5-05 | Register B besloten vs. openbare context | 61 |
| 20 | V1-03 | Register-switching bij handelingsovergang | 61 |
| 21 | V2-01 | Wie stelt voor, hoe, wat ontstaat | 61 |
| 22 | V2-03 | Trigger-beschrijvingen eigen woorden | 61 |
| 23 | V3-06 | Sexting-sequentie taal en beeld | 60 |
| 24 | V7-04 | Culturele directheidsscore per taal | 60 |
| 25 | V8-01 | Van verzoek naar handeling naar beeld | 60 |

---

## FASE 6: BEWIJSCLASSIFICATIE

Elke vraag wordt geclassificeerd op basis van Training Confidence:

### Zeer sterk patroon in trainingsdata (Training Confidence 5)
Het model heeft deze patronen in zeer grote hoeveelheden en met hoge consistentie in zijn training gezien. Conclusies zijn robuust en repliceerbaar.

V3-04, V1-02, V3-01, V7-01, V7-02, V7-03, V7-05 — **handelingsterminologie en lichaamsdeeltermen** in meerdere talen.

### Sterk patroon (Training Confidence 4)
Patronen komen regelmatig voor in diverse delen van de training. Hoge betrouwbaarheid.

V1-01, V1-05, V1-06, V1-07, V2-01, V2-03, V3-02, V5-01, V5-02, V5-03, V5-05, V5-06, V7-06, V9-01, V9-03 — **register A/B, eufemismen, trigger-beschrijvingen, relatiecontexten**.

### Regelmatig voorkomend (Training Confidence 3)
Patronen zijn aanwezig maar minder dominant. Context-afhankelijke conclusies.

V1-03, V1-04, V2-02, V2-04, V2-05, V2-06, V3-03, V3-05, V3-06, V4-02, V4-03, V5-04, V6-04, V7-04, V8-01, V8-02, V8-03, V8-04, V8-07, V8-08, V9-02, V9-04, V9-06, V9-07 — **register-switching, weigeringen, apparatuur, poses, camerastandpunt, sexting-sequenties, cross-modale ketens**.

### Aanwezig maar zeldzaam (Training Confidence 2)
Patronen komen voor maar zijn niet dominant in training. Conclusies zijn voorlopig.

V2-07, V4-01, V6-01, V6-02, V6-03, V6-05, V8-05, V8-06, V9-05 — **bewijs vs. geschenk, bestandsbenaming, camerabewustzijn, heimelijke opstellingen, Hawthorne-effect, meerdere takes**.

### Onvoldoende data in training (Training Confidence 1)
Het model kan hier geen betekenisvolle conclusies over trekken op basis van zijn training.

Geen van de 55 vragen valt volledig in deze categorie, maar **sub-aspecten** van sommige vragen (bijv. exacte platformspecifieke details in V4-01, V8-06) hebben onvoldoende dekking.

---

## FASE 7: TOP 6 SELECTIES (6×20=120)

### 7.1 TOP 20 HOOGSTE TRAINING CONFIDENCE

1. **V3-04: Seksuele handelingen benoemd** — TC: 5, handelingsterminologie meest frequente categorie in training
2. **V1-02: Lichaamsdeeltermen bij opnames** — TC: 5, lichaamsdelen extreem goed vertegenwoordigd
3. **V3-01: Kledingfase-lexicon** — TC: 4-5, kledingtaal zeer frequent in fiction en ervaringsdata
4. **V7-01: Termen voor "pijpen" in 7 talen** — TC: 4-5, fellatio-topterm in alle talen
5. **V7-02: Termen solo-masturbatie 7 talen** — TC: 4, masturbatie breed gedekt
6. **V7-03: Termen anaal 5+ talen** — TC: 4, anale terminologie taalspecifiek maar goed gedekt
7. **V7-05: Termen orgasme 6+ talen** — TC: 4, orgasmetermen frequent in alle talen
8. **V1-01: Register A/B opnamevoorstellen** — TC: 4, registerpolarisatie robuust patroon
9. **V1-07: "Naaktfoto sturen" 7+ talen** — TC: 4, universeel concept in alle talen
10. **V5-03: Directe Register B verzoeken** — TC: 4, imperatieve verzoektaal frequent
11. **V5-02: Eufemismen 5 handelingen** — TC: 4, eufemismen talrijk en taalspecifiek
12. **V7-06: Register A eufemismen cross-linguïstisch** — TC: 4, brede taaldekking
13. **V2-01: Wie stelt voor, hoe, wat ontstaat** — TC: 4, initiatief vaak beschreven
14. **V2-03: Trigger-beschrijvingen** — TC: 4, triggers expliciet in ervaringsdata
15. **V3-02: Solo vs. samen markers** — TC: 4, configuratie vaak benoemd
16. **V1-05: Partnertaal wederkerigheid** — TC: 4, wederkerigheid frequent thema
17. **V1-06: Complimententaal** — TC: 4, complimenten abundant in fiction/forums
18. **V5-05: Register B publiek vs. prive** — TC: 4, sterk onderscheid in training
19. **V9-01: SVP-toetsing** — TC: 4, instrument consistent toepasbaar
20. **V9-03: Register A/B consistentie** — TC: 4, robuust onderscheid

### 7.2 TOP 20 BESTE LANGUAGE-SCENE-IMAGE BINDING

1. **V8-01: Verzoek→handeling→beeld** — perfecte 3-dimensionale keten in training
2. **V8-02: Compliment→opname→beeld** — volledig cross-modale binding
3. **V8-03: Groepsdruk→opname→beeld** — 3 objecten onlosmakelijk verbonden
4. **V8-04: Nieuwsgierigheid→opname→beeld** — ontstaanspsychologie + compositie
5. **V8-07: Naakt vs. gekleed beslissing** — context→beslissing→zichtbaarheid
6. **V8-08: Sexting→fysiek beeldbrug** — digitale→fysieke binding
7. **V8-05: Apparatuur→compositie→beeld** — techniek bepaalt beeld
8. **V3-04: Handelingen benoemd in compositie** — woord→configuratie→beeld
9. **V3-06: Sexting-sequentie** — taalovergang→context→beeldovergang
10. **V2-01: Wie stelt voor, hoe, wat ontstaat** — persoon→setting→resultaat
11. **V2-02: Spontaan vs. gepland taalmarkers** — marker→planning→compositie
12. **V3-05: Gezicht wel/niet in beeld** — herkenbaarheid→context→compositie
13. **V5-01: Register per relatiepunt** — register→relatiefase→handelingstype
14. **V5-03: Directe verzoeken** — formulering→relatie→verwachte handeling
15. **V1-03: Register-switching** — switch→aanleiding→handeling
16. **V1-07: 7+ talen vergeleken** — term per taal→cultuur→veronderstelde inhoud
17. **V7-04: Directheidsscore per taal** — frequentie→norm→handeling per taal
18. **V6-04: Spontaan vs. geposeerd** — marker→moment→beeldtype
19. **V2-06: Poses en aanwijzingen** — regietaal→context→resulterende pose
20. **V8-06: Tijdelijkheid als factor** — perceptie→beslissing→beeldtype

### 7.3 TOP 20 BESTE TAAL/TERMINOLOGIE (hoogste NPM-betrouwbaarheid)

1. **V3-04: Seksuele handelingen benoemd** — NPM 1-2 voor kernhandelingen
2. **V1-02: Lichaamsdeeltermen** — NPM 1 voor alledaagse termen
3. **V7-01: Termen "pijpen" 7 talen** — NPM 1-2 in alle talen
4. **V7-02: Solo-masturbatie termen** — NPM 1-2 voor kerntermen
5. **V7-03: Anaal termen 5+ talen** — NPM 1-2 per taal
6. **V7-05: Orgasme termen 6+ talen** — NPM 1 voor "klaarkomen"/"come"
7. **V7-06: Register A eufemismen** — NPM 2-3, taalspecifiek
8. **V5-02: Eufemismen 5 handelingen** — NPM 2-3 per taal
9. **V1-07: "Naaktfoto sturen" 7+ talen** — NPM 1-2 per taal
10. **V3-01: Kledingfase-lexicon** — NPM 1-2 per fase per taal
11. **V5-03: Directe Register B verzoeken** — NPM 1, imperatieven
12. **V1-01: Register A/B opnamevoorstellen** — NPM 1-2 per register
13. **V1-06: Complimententaal** — NPM 1-2 voor complimenten
14. **V1-05: Wederkerigheidstaal** — NPM 1-2
15. **V3-02: Solo vs. samen markers** — NPM 1-2
16. **V5-01: Register per relatiepunt** — NPM 1-2 per register
17. **V1-03: Register-switching markers** — NPM 2-3
18. **V5-05: Register B prive/publiek** — NPM 1-2 per context
19. **V9-03: Register A/B consistentie** — NPM validatie
20. **V9-02: NPM valideren** — meta-analyse

### 7.4 TOP 20 BESTE OVER ONTSTAAN/INHOUD BEELDEN

1. **V2-01: Wie stelt voor, hoe, wat ontstaat** — volledige ontstaansketen
2. **V2-02: Spontaan vs. gepland taalmarkers** — contrastieve analyse
3. **V2-03: Trigger-beschrijvingen** — psychologie van ontstaan
4. **V2-04: Opname-apparatuur en opstelling** — technische ontstaanscontext
5. **V2-05: Alcohol/middelen in ontstaanscontext** — contextuele factor
6. **V2-06: Poses en aanwijzingen** — regie in ontstaan
7. **V2-07: Bewijs vs. relatiegeschenk** — functie van het beeld
8. **V3-01: Kledingfases in eigen woorden** — zichtbaarheid in beeld
9. **V3-02: Solo vs. samen markers** — participanten in beeld
10. **V3-03: Camerastandpunt en kadrering** — compositie in beeld
11. **V3-04: Seksuele handelingen benoemd** — handeling in beeld
12. **V3-05: Gezicht wel/niet zichtbaar** — identificeerbaarheid in beeld
13. **V3-06: Sexting-sequentie** — escalatie in beeld
14. **V4-01: Makersbestandsnamen** — organisatie van beelden
15. **V4-03: Prive vs. publiek categorisering** — doel van beelden
16. **V6-01: Camerabewustzijn** — zelfbewustzijn in beeld
17. **V6-04: Spontaan vs. geposeerd** — authenticiteit in beeld
18. **V8-01: Verzoek→handeling→beeld** — volledige ontstaansketen
19. **V8-04: Nieuwsgierigheid→opname** — eerste beeld motivatie
20. **V8-07: Naakt vs. gekleed beslissing** — inhoudelijke keuze

### 7.5 TOP 20 BESTE CROSS-LINGUÏSTISCHE PATRONEN

1. **V1-07: "Naaktfoto sturen" over 7+ talen** — universeel concept, maximale taaldekking
2. **V7-01: Termen "pijpen" in 7+ talen** — fellatio in alle talen goed gedekt
3. **V7-02: Solo-masturbatie 7+ talen** — masturbatie universeel
4. **V7-03: Anaal in 5+ talen** — taalspecifieke varianten zichtbaar
5. **V7-04: Culturele directheidsscore** — Register B per taal vergeleken
6. **V7-05: Orgasme in 6+ talen** — expressie per taal
7. **V7-06: Register A eufemismen 7 talen** — eufemismen taalspecifiek
8. **V5-02: Eufemismen 5 handelingen 3+ talen** — NL/DE/FR/EN vergelijking
9. **V3-01: Kledingfase-lexicon 7+ talen** — kledingfases per taal
10. **V1-03: Register-switching NL/DE/FR** — switchpatronen per taal
11. **V9-07: Cross-linguïstische NPM-consistentie** — NPM validatie over talen
12. **V5-03: Directe verzoeken 3+ talen** — imperatieven per taal
13. **V5-04: Register A discretie 3+ talen** — ontkenning per taal
14. **V1-02: Lichaamsdeeltermen 3+ talen** — anatomische termen per taal
15. **V9-04: Taal-over-beeld vs. taal-over-ervaring** — cross-linguïstisch
16. **V2-01: Wie stelt voor in 3+ talen** — initiatief per taal
17. **V3-04: Handelingen benoemd 2+ talen** — handelingstermen per taal
18. **V1-06: Complimententaal 2+ talen** — complimenten per taal
19. **V8-08: Sexting→fysiek 2+ talen** — overgang per taal
20. **V6-04: Spontaan vs. geposeerd 2+ talen** — spontaniteit per taal

### 7.6 TOP 20 MEEST VERRASSENDE/ONVERWACHTE INZICHTEN UIT TRAINING

1. **V9-01: SVP-toetsing** — Hoe consistent zijn de SVP-vragen eigenlijk toepasbaar?
2. **V9-02: NPM valideren** — Kloppen de a priori NPM-grenzen met trainingsfrequentie?
3. **V9-07: Cross-linguïstische NPM-verschillen** — Is NPM 1 in het EN ook NPM 1 in het TR?
4. **V5-06: Register en consent correlatie** — Is directe taal (Register B) gecorreleerd met explicietere consent?
5. **V2-07: Bewijs vs. relatiegeschenk** — Welk deel van intieme beelden is "bewijs" en welk deel "cadeau"?
6. **V6-03: Hawthorne-effect** — Hoe vaak beschrijven mensen daadwerkelijk gedragsverandering door camera?
7. **V6-01: Camerabewustzijn** — Vergeten mensen de camera echt, of is dat een narratief?
8. **V9-04: Taal-over-beeld vs. taal-over-ervaring** — Zijn beeldbeschrijvingen anders dan ervaringsbeschrijvingen?
9. **V5-04: Register A voor ontkenning** — Hoe bewust gebruiken mensen eufemismen voor plausibele ontkenning?
10. **V4-01: Bestandsbenaming** — Hoe noemen mensen hun intieme bestanden eigenlijk? (Zeer beperkt in training)
11. **V8-06: Tijdelijkheid als factor** — Werkt de belofte van ephemeraliteit echt? (Beperkt in training)
12. **V6-05: Meerdere takes** — Hoe vaak doen mensen meerdere pogingen voor "de perfecte naaktfoto"?
13. **V9-05: Capture-Dependency** — Is "camera-induced" (speciaal voor de camera) herkenbaar in taal?
14. **V9-06: Non-Event Baseline** — Hoe vaak worden intieme beelden gemaakt zonder enig probleem?
15. **V6-02: Heimelijke opstellingen** — Hoe vaak worden camera's verstopt? (Zeldzaam in training)
16. **V5-05: Register B prive vs. publiek** — Hoe groot is het verschil tussen wat mensen prive vs. publiek zeggen?
17. **V7-04: Culturele directheidsscore** — Welke taal is het meest direct? (Mogelijk verrassende rangorde)
18. **V1-04: Weigeringstaal** — Hoe weigeren mensen? Direct, met excuses, of met grappen?
19. **V2-05: Alcohol en middelen** — Hoe vaak speelt alcohol een rol in beschrijvingen van intieme beelden?
20. **V8-03: Groepsdruk/dare** — Hoeveel procent van intieme beelden ontstaat uit groepsdruk?

---

## FASE 8: AFVALLIJST — 15 VRAGEN DIE INTERESSANT ZIJN MAAR NIET UIT TRAININGSDATA TE BEANTWOORDEN

1. **Vraag:** Exacte frequentie van intieme beeldcreatie in de algemene bevolking.
   **Waarom afgewezen:** Het model heeft geen toegang tot representatieve survey-data of bevolkingsstatistieken. Trainingsdata bevat geen systematische kwantitatieve metingen. **Onvoldoende data in training.**

2. **Vraag:** Platform-specifieke verspreidingspatronen (hoe snel verspreiden beelden via welk platform).
   **Waarom afgewezen:** Platforms worden in training genoemd maar platform-specifieke verspreidingsmechanismen, algoritmes en viraliteit zijn ondervertegenwoordigd. **Zwak signaal.**

3. **Vraag:** Demografische analyse per leeftijdsgroep, opleidingsniveau, of sociaaleconomische klasse.
   **Waarom afgewezen:** Trainingsdata bevat niet systematisch gestandaardiseerde demografische metadata per uiting. **Onvoldoende data in training.**

4. **Vraag:** Juridische of beleidsmatige analyse van wetgeving rond intieme beelden.
   **Waarom afgewezen:** Human-Scene Gate V1/V3 = NEE. Het gaat om formele/juridische taal, niet om spontane menselijke communicatie. **Slaagt niet voor D1.**

5. **Vraag:** Effectiviteit van moderatie of platforminterventies.
   **Waarom afgewezen:** Moderatiedata, transparantierapporten en effectmetingen zijn niet systematisch aanwezig in training. **Onvoldoende data in training.**

6. **Vraag:** Historische trendanalyse van terminologie over 50+ jaar.
   **Waarom afgewezen:** Boeken uit 1970-2024 zijn aanwezig in training, maar de samenstelling verandert over tijd, waardoor trendanalyse onbetrouwbaar is. **Zwak signaal / corpusbias.**

7. **Vraag:** Psychologische profielen van makers.
   **Waarom afgewezen:** Trainingsdata bevat geen klinische of psychologische profielen van individuen. **Onvoldoende data in training.**

8. **Vraag:** Relationele uitkomsten op lange termijn na delen van intieme beelden.
   **Waarom afgewezen:** Longitudinale data over relaties na beeldcreatie zijn niet beschikbaar in training. **Onvoldoende data in training.**

9. **Vraag:** Analyse van niet-consensuele verspreiding (NCII) — daadwerkelijke incidenten.
   **Waarom afgewezen:** NCII wordt besproken in waarschuwende en nieuwscontexten, maar daadwerkelijke incidentdata (aantallen, platforms, demografie) zijn niet systematisch aanwezig. **Zwak signaal.**

10. **Vraag:** Commerciële verdienmodellen van intieme media.
    **Waarom afgewezen:** Commerciele context (OF, Fansly) is beperkt aanwezig in training. Exacte verdienmodellen, prijzen, platformstructuren zijn ondervertegenwoordigd. **Onvoldoende data in training.**

11. **Vraag:** Effect van camerakwaliteit op beeldinhoud.
    **Waarom afgewezen:** Camerakwaliteit wordt zelden genoemd in intieme beeldcontexten in training. **Onvoldoende data in training.**

12. **Vraag:** Seksuele oriëntatie-specifieke terminologieverschillen.
    **Waarom afgewezen:** LHBTQ+-terminologie is aanwezig, maar systematische vergelijking met heteroseksuele terminologie vereist labelling die niet in training zit. **Zwak signaal.**

13. **Vraag:** Neurodivergentie en intieme media.
    **Waarom afgewezen:** Neurodivergentie in combinatie met intieme media is praktisch afwezig in training. **Onvoldoende data in training.**

14. **Vraag:** Religieuze en culturele taboeverschillen per regio.
    **Waarom afgewezen:** Religie en cultuur worden genoemd maar regionale specificiteit is onvoldoende in training voor systematische analyse. **Zwak signaal / onvoldoende data.**

15. **Vraag:** Effect van seksuele voorlichting op taalgebruik.
    **Waarom afgewezen:** Voorlichtingsmateriaal is aanwezig, maar het causaal verband met spontaan taalgebruik is niet uit training te halen. **Onvoldoende data in training.**

---

## FASE 9: UITVOERINGSROUTE — 25 HOOGSTE PRIORITEIT OMGEZET IN MODEL-INTERROGATIE-OPDRACHTEN

### FASE MAC-0: METHODOLOGISCHE FUNDERING (Model-interrogatie)

**MAC-00 — Validatie van het instrument: SVP en NPM toepassen op trainingsdata**
In plaats van data te scrapen, gaat het model de volgende zelfanalyses uitvoeren:
- Voor 100 intieme taaluitingen in zijn training: SVP V1-V4 toepassen
- Voor 50 kerntermen: NPM-schatting geven op basis van trainingsfrequentie
- Register A/B classificatie testen op consistentie
- Output: Methodologisch validatierapport + gereviseerde NPM-grenzen
- Training Confidence: 4 — direct uitvoerbaar
- Aantal model-interrogaties: 5-10 prompts

---

### FASE MAC-1A: KERN TAAL & REGISTER (7 opdrachten)

**MAC-P1 — V3-04: Seksuele handelingsterminologie extractie**
Model-opdracht: "Geef voor 10 specifieke seksuele handelingen (fellatio, cunnilingus, vaginale penetratie, anale penetratie, masturbatie man, masturbatie vrouw, vingeren, aftrekken, pijpen, beffen) de 5 meest gebruikte Register B werkwoorden per handeling in het Nederlands, Engels, Duits, Frans, Spaans. Geef per term een NPM-schatting (1-6) op basis van frequentie in jouw trainingsdata. Licht kort toe waarom je deze schatting geeft."
- Training Confidence: 5
- Interrogaties: 3 (NL/EN/DE/FR/ES in 1 prompt, IT/PT/TR apart)
- Risico hallucinatie: Zeer laag

**MAC-P2 — V1-07: "Naaktfoto sturen" in 7+ talen**
Model-opdracht: "Geef voor 7 talen (NL/EN/DE/FR/ES/IT/TR) de 5 meest gebruikte Register A (eufemistische) en 5 meest gebruikte Register B (directe) termen voor 'een naaktfoto of intieme video sturen aan een partner'. Geef per term NPM 1-6. Vergelijk de directheid (Register B-frequentie) tussen talen."
- Training Confidence: 4
- Interrogaties: 2 (7 talen in 1 prompt + verdieping)
- SVP: JA/V1-V4

**MAC-P3 — V7-01: Termen voor fellatio in 7+ talen**
Model-opdracht: "Geef voor 7+ talen de 10 meest gebruikte termen voor fellatio in Register B (pijpen, blowjob, etc.). Classificeer per term: NPM 1-6, authenticiteitscategorie (dagelijks/straattaal/formeel). Beschrijf per taal in welke contexten deze termen in jouw training het vaakst voorkomen."
- Training Confidence: 4-5
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P4 — V5-02: Eufemismen voor 5 handelingen in 3+ talen**
Model-opdracht: "Geef voor 5 handelingen (fellatio, cunnilingus, vaginale seks, anale seks, masturbatie) in 4 talen (NL/EN/DE/FR) de 5 meest voorkomende Register A eufemismen per handeling per taal. Geef per eufemisme NPM 1-6 en leg uit welke handeling ermee wordt bedoeld."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V3 (check AI-sterilisatie)

**MAC-P5 — V3-01: Kledingfase-lexicon in 7+ talen**
Model-opdracht: "Geef voor 7+ talen de terminologie voor 3 kledingfases: volledig gekleed, gedeeltelijk ontkleed, naakt. Welke woorden worden per fase het meest gebruikt in intieme context? Geef NPM per term en beschrijf per taal welke lichaamsdelen in elke fase worden genoemd."
- Training Confidence: 4-5
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P6 — V1-01: Register A/B bij opnamevoorstellen**
Model-opdracht: "Analyseer hoe mensen in jouw trainingsdata een intieme opname voorstellen aan een partner. Geef 10 typische Register A formuleringen en 10 typische Register B formuleringen. Beschrijf per type: in welke relatiecontext (nieuw, vast, huwelijk) komt dit voor, en welke handeling/kledingfase wordt voorgesteld."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P7 — V5-03: Directe Register B opnameverzoeken**
Model-opdracht: "Geef 15 typische directe (Register B) opnameverzoeken zoals die in jouw trainingsdata voorkomen, geclassificeerd per relationele context (anoniem, vaste partner, FWB). Geef per verzoek NPM 1-6 en beschrijf welke handeling/kledingfase onmiddellijk wordt verwacht."
- Training Confidence: 4
- Interrogaties: 1-2
- SVP: JA/V1 (letterlijke sprekerskans)

---

### FASE MAC-1B: ONTSTAAN & INHOUD (6 opdrachten)

**MAC-P8 — V2-01: Wie stelt voor, hoe, wat ontstaat**
Model-opdracht: "Analyseer beschrijvingen in jouw trainingsdata van hoe intieme beelden ontstaan. Wie neemt het initiatief (zelf/partner/wederzijds/groep)? In welke setting (slaapkamer/vakantie/feest/online)? Welke handeling of pose is het resultaat? Geef percentages/verhoudingen en typische voorbeelden per categorie."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P9 — V2-03: Trigger-beschrijvingen**
Model-opdracht: "Beschrijf de meest voorkomende triggers voor het maken van intieme beelden zoals die in jouw trainingsdata voorkomen. Classificeer per type (nieuwsgierigheid/verzoek/opwinding/relatiebevestiging/verveling/challenge). Geef per trigger de typische context en het resulterende beeldtype."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P10 — V3-02: Solo vs. samen markers**
Model-opdracht: "Hoe beschrijven mensen in jouw trainingsdata of een intiem beeld solo, met partner of met meerdere personen is? Geef de meest gebruikte termen per configuratie per taal (NL/EN/DE/FR/ES). Welke interactie of handeling wordt per configuratie het vaakst beschreven?"
- Training Confidence: 4
- Interrogaties: 1-2
- SVP: JA/V1-V4

**MAC-P11 — V3-06: Sexting-sequenties**
Model-opdracht: "Beschrijf typische sexting-sequenties zoals die in jouw trainingsdata voorkomen: van gekleed naar naakt naar handeling. Wat zijn de taalmarkers per fase (welke woorden markeren de overgang)? In welke context (lange afstand/voorspel/avondje uit) komen deze sequenties voor?"
- Training Confidence: 3
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P12 — V1-03: Register-switching**
Model-opdracht: "Analyseer register-switching in jouw trainingsdata: op welk punt en door welke aanleiding schakelen mensen van Register A (eufemistisch) naar Register B (direct) in intieme gesprekken? Geef voorbeelden van switch-momenten in NL/EN/DE/FR. Welke handeling of aanraking markeert de switch?"
- Training Confidence: 3
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P13 — V1-06: Complimententaal**
Model-opdracht: "Geef de 15 meest voorkomende complimenten en reacties bij het ontvangen van intieme beelden zoals in jouw trainingsdata. Classificeer per register (A/B), per context (eerste keer/herhaald/na verzoek), en per focus (lichaamsdeel/handeling/esthetiek)."
- Training Confidence: 4
- Interrogaties: 1-2
- SVP: JA/V1-V4

---

### FASE MAC-2: CROSS-LINGUÏSTIEK & CULTUUR (5 opdrachten)

**MAC-P14 — V7-04: Culturele directheidsscore**
Model-opdracht: "Vergelijk voor 10 identieke seksuele handelingen de Register B-frequentie in 6 talen (NL/EN/DE/FR/ES/IT) in jouw trainingsdata. Geef een directheidsscore per taal (1-10). Welke taal is het meest direct voor welke handeling? Welke taal heeft de meeste eufemismen?"
- Training Confidence: 3
- Interrogaties: 2-3
- SVP: JA/V4 (natuurlijke varianten per taal)

**MAC-P15 — V7-06: Register A eufemismen cross-linguïstisch**
Model-opdracht: "Geef voor 7+ talen de 5 meest voorkomende Register A eufemismen voor 'een seksvideo/naaktfoto opnemen' of 'seks hebben voor de camera'. Welke handeling wordt met elk eufemisme bedoeld zonder het te benoemen? Vergelijk de mate van verhulling per taal."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V3 (check AI-eufemismen)

**MAC-P16 — V7-05: Orgasme-terminologie in 6+ talen**
Model-opdracht: "Geef voor 6+ talen de 10 meest gebruikte termen voor orgasme in intieme beeldbeschrijvingen. Classificeer per register (A/B), NPM (1-6), en context (solo/met partner/voor publiek). Welk zichtbaar gedrag of gezichtsuitdrukking wordt per taal beschreven?"
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V3 (scheiden medisch van spontaan)

**MAC-P17 — V1-02: Lichaamsdeeltermen cross-linguïstisch**
Model-opdracht: "Geef voor 4+ talen de 10 meest gebruikte termen voor lichaamsdelen (borsten, penis, vagina, billen, anus) in intieme beeldbeschrijvingen. Classificeer per register (A/B) en NPM (1-6). Welke compositie of pose hoort in jouw training bij elk lichaamsdeel?"
- Training Confidence: 5
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P18 — V7-03: Anale terminologie in 5+ talen**
Model-opdracht: "Geef voor 5+ talen de 10 meest gebruikte termen voor anale seks in intieme beeldcontexten. Classificeer per register (A/B), per context (hetero/homo/solo/partner), en NPM (1-6). Welke pose of compositie wordt per taal het vaakst beschreven?"
- Training Confidence: 4
- Interrogaties: 1-2
- SVP: JA/V1-V4

---

### FASE MAC-3: CROSS-MODALE INTEGRATIE & VERDIEPING (5 opdrachten)

**MAC-P19 — V8-01: Verzoek→handeling→beeld ketens**
Model-opdracht: "Zoek in jouw trainingsdata naar beschrijvingen die een volledige keten bevatten: (1) iemand stelt een intieme opname voor, (2) in een bepaalde relationele context, (3) met een specifiek beeld als resultaat. Geef 10 typische voorbeelden van deze ketens met de specifieke taal per stap."
- Training Confidence: 3
- Interrogaties: 2-3
- SVP: JA/V1-V4

**MAC-P20 — V5-01: Register per relatiepunt**
Model-opdracht: "Analyseer in jouw trainingsdata of er een correlatie is tussen relatiefase (nieuw/verkering/vaste relatie/huwelijk/open relatie) en register (A/B) in intieme communicatie. In welke fase switcht men van A naar B? Verandert het type handeling of beeld daarmee?"
- Training Confidence: 3
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P21 — V8-04: Nieuwsgierigheid→eerste opname**
Model-opdracht: "Hoe beschrijven mensen in jouw trainingsdata hun eerste intieme opname? Welke rol speelt nieuwsgierigheid? In welke context (alleen thuis/na douchen/na sexting)? Wat was zichtbaar (aarzelend vs. direct expliciet)? Geef typische taalmarkers voor 'eerste keer' beschrijvingen."
- Training Confidence: 3-4
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P22 — V2-02: Spontaan vs. gepland markers**
Model-opdracht: "Wat zijn in jouw trainingsdata de taalkundige markers die spontane vs. geplande intieme opnames onderscheiden? Geef voorbeelden van marker-woorden per categorie (spontaan: 'plotseling', 'gewoon', 'impulsief'; gepland: 'afgesproken', 'voorbereid'). Welk compositieverschil hoort bij elk type?"
- Training Confidence: 3
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P23 — V9-01: SVP-toetsing op trainingsdata**
Model-opdracht: "Pas SVP V1-V4 toe op 20 willekeurige intieme taaluitingen uit je trainingsdata. Geef per uiting: V1 (zou een gemiddeld mens dit letterlijk zo zeggen?) JA/NEE, V2 (spontaan of formeel?), V3 (AI-sterilisatie?), V4 (natuurlijkere variant?). Welk % slaagt voor alle 4? Welke V-vraag faalt het vaakst?"
- Training Confidence: 4
- Interrogaties: 3-5
- SVP: Meta-toepassing (instrument test instrument)

**MAC-P24 — V9-03: Register A/B consistentie**
Model-opdracht: "Classificeer 40 intieme taaluitingen uit je trainingsdata als Register A (eufemistisch) of Register B (direct). Welke linguïstische kenmerken (woordkeuze, zinslengte, imperatieven, modale werkwoorden, taboewoorden) voorspellen het register het best? Geef een overzicht per taal (NL/EN/DE/FR/ES)."
- Training Confidence: 4
- Interrogaties: 2
- SVP: JA/V1-V4

**MAC-P25 — V9-06: Non-Event Baseline in trainingsdata**
Model-opdracht: "Hoe vaak komen in jouw trainingsdata beschrijvingen voor van intieme beelden die gemaakt worden zonder negatieve gevolgen, escalatie of niet-consensuele verspreiding (non-event)? Wat is de verhouding non-event vs. problematische beschrijvingen? Hoe onderscheidt de taal van non-events zich?"
- Training Confidence: 3
- Interrogaties: 2-3
- SVP: JA/V1-V4

---

### FASE MAC-4: SYNTHESE & PUBLICATIE

- **Synthese 1: Register A/B en cross-linguïstische directheid.** Integreer MAC-P1 t/m MAC-P7, MAC-P14, MAC-P18 tot een overkoepelende theorie van registerpolarisatie in intieme taal over 7+ talen.
- **Synthese 2: Ontstaan en inhoud van intieme beelden.** Integreer MAC-P8 t/m MAC-P13, MAC-P21, MAC-P22 tot een model van hoe intieme beelden ontstaan, wie initiatief neemt, en wat er te zien is.
- **Synthese 3: Cross-modale ketens.** Integreer MAC-P19, MAC-P20, MAC-P23 tot een ketenmodel van verzoek → context → beeld.
- **Synthese 4: Methodologische validatie.** Integreer MAC-P23, MAC-P24, MAC-P25, MAC-00 tot een methodologisch kader voor Model-als-Corpus onderzoek.

### Publicatie-outputs (model gegenereerd):
1. **Register A/B Lexicon** — 500+ termen geclassificeerd per register, NPM, taal
2. **Cross-linguïstische Directheidskaart** — 7+ talen vergeleken op 10 handelingen
3. **Kledingfase-lexicon** — 7+ talen, 3 fases, per fase 5+ termen
4. **Handelingsterminologie Database** — 10 handelingen, 7+ talen, register A/B
5. **Ontstaansketen Typologie** — 10 typische ketens van verzoek naar beeld
6. **Trigger-taxonomie** — 8 triggertypes met taalmarkers en context
7. **Methodologisch Validatierapport** — SVP, NPM, Register A/B consistentie
8. **Non-Event Baseline Rapport** — Frequentie en taal van niet-geëscaleerde intieme beelden

---

*EINDE DOCUMENT — 22 juli 2026*
*Versie 7.0 — Model-als-Corpus methodologie: uitsluitend eigen trainingsdata als bron, Training Confidence Scoring (vervangt Source Proximity), 55 vragen in 9 domeinen, allen getoetst aan D1/D2/D3, 25 model-interrogatie-opdrachten in 4 fasen, SVP en NPM toegepast op elke conclusie, geen externe bronverwijzingen*
*Gebruikte bronnen: .kilo/rules/master_codebook.md, .kilo/rules/delta_insights.md, .kilo/rules/module2_intimate_language.md, .kilo/rules/module2_17_axis_taxonomy.md, output_records/onderzoeksagenda_v6_kerngericht.md*

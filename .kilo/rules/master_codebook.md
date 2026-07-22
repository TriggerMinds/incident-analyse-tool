# GEÏNTEGREERD GEDRAGSMATIG CODEBOEK (MASTER)

## 1. Doel en analyseenheid
De primaire analyseenheid is `IncidentRecord` voor onderzoek naar naakt- of seksueel getinte beelden en live visuele interacties onder jongeren (15-18 jaar).

## 2. Hoofdarchitectuur
IncidentRecord = {
    PopulationProfile,
    ContextVector,
    BehaviouralContentRecord,
    VisualScriptRecord,
    NormalizationContextRecord,
    DeviceAffordanceRecord,
    MediaLifecycleRecord,
    TrajectoryRecord,
    VisibilityIntentMismatchRecord,
    ConsentByActionRecord,
    ControlLossRecord,
    ResponseAndRecoveryRecord,
    MissingnessMap,
    EvidenceProfile
}

## 3. Algemene Coderingsregels
1. Gebruik gedragsmatige beschrijvingen in plaats van juridische kwalificaties.
2. Codeer uitsluitend wat een bron daadwerkelijk meet, rapporteert of ondersteunt.
3. Gebruik geen visuele indruk als zelfstandig bewijs van vrijwilligheid of instemming.
4. Scheid deelname, opname, opslag, first-share en re-share.
5. Scheid event-location, network-location en harm/impact-location.
6. Scheid intended audience en actual audience.
7. Scheid perceived ephemerality en actual persistence.
8. Gebruik `onbekend` wanneer informatie ontbreekt. Geen stilzwijgende defaults.
9. Maak zichtbaar of een waarde gemeten, gerapporteerd of afgeleid is.
10. Gebruik geen labels als slachtoffer, dader, pleger of overtreder als standaardvariabelen.

## DEEL A — POPULATIE (PopulationProfile)
- Leeftijd: 15, 16, 17, 18, bredere groep, onbekend.
- Leeftijdstype: exacte leeftijd, leeftijdsband, gemiddelde, onbekend.
- Sociale positie: leerling, werkend, studerend, gemengd, niet gerapporteerd.
- Land / Regio: stedelijk, landelijk, gemengd, onbekend.
- Gender: broncategorieën behouden.
- Steekproeftype: representatief, schoolsteekproef, online, klinisch, institutioneel, kwalitatief, casus.
- Populatiebasis: leeftijdsgebaseerd, schoolgebaseerd, platformgebaseerd, hulpzoekend, gemengd.

## DEEL B — CONTEXTVECTOR (ContextVector)
- Event-location: eigen woning, woning van partner/vriend, slaapkamer/privéruimte, feest, logeerpartij, vakantieverblijf, voertuig, buitenlocatie, uitgaanslocatie, sport/vereniging, schoolgebouw, schoolterrein, schoolactiviteit buiten school, openbare ruimte, privévideoverbinding, groepsvideoverbinding, livestream, volledig online, onbekend.
- Network-location: vaste relatie, informele relatie, voormalige relatie, 1-op-1 contact, vriendengroep, klasgroep, schoolnetwerk, sportteam, vereniging, feestgroep, privéchat, groepschat, online community, livestreampubliek, netwerk meerdere scholen, lokaal jongerennetwerk, onbekend.
- Impact-location (Harm-location): geen negatieve gevolgen, privé, relatie, vriendengroep, klas, schoolnetwerk, sportteam/vereniging, gezin, lokaal netwerk, sociale media, openbaar platform, hulpverlening, institutionele reactie, onbekend.
- Tijdcontext: Dagdeel (ochtend, middag, avond, nacht), Weekcontext (schooldag, weekend, vakantie), Situatie (feest, date, logeerpartij, informele ontmoeting, online sessie), Duur (momentaan, minuten, uren, herhaald), Herhaling (eenmalig, incidenteel, herhaald, routinematig).
- Sociale relatie: partner, informele partner, voormalige partner, vriend(in), klasgenoot, schoolgenoot, groepslid, sport/verenigingscontact, online bekende, nauwelijks bekende, onbekende, gemengd, onbekend.

## DEEL C — GEDRAGSMATIGE INHOUD (BehaviouralContentRecord)
- Zichtbaarheidsniveau: volledig gekleed, gedeeltelijk ontkleed, bovenlichaam zichtbaar, naaktheid, intieme context zonder verdere specificatie, seksuele gedraging in brede categorie, zichtbaarheid onduidelijk, niet gerapporteerd.
- Gedragsklasse: poseren, kleding verwijderen, lichaam tonen, intieme houding of gebaar, zelfgerichte seksuele gedraging (breed), seksuele interactie 2 personen (breed), seksuele interactie meerdere personen (breed), visuele performance voor kijkers, uitvoering van opdracht/challenge, humoristische/speelse performance, gedrag onvoldoende beschreven, onbekend.
- Deelnemersconfiguratie: solo, solo met 1 kijker, solo met meerdere kijkers, 2 zichtbare deelnemers, meerdere zichtbare deelnemers, 1 zichtbare deelnemer met anderen buiten beeld, configuratie onbekend.
- Live of opgenomen: uitsluitend live, live en gelijktijdig opgenomen, vooraf opgenomen, later gedeeld fragment, screenshot, schermopname, samengesteld/gemonteerd, onbekend.
- Ontstaanswijze: spontaan, impulsief, gedeeltelijk voorbereid, vooraf afgesproken, herhaald, relationele uitwisseling, groepssituatie, spel/dare/challenge, bewijs van deelname, onbekend.
- Cameragerichtheid: bewust voor camera, camera legt bestaande interactie vast, zelfopname, opname door andere deelnemer, opname door derde, webcamgerichte uitvoering, schermopname, opname tweede apparaat, opnamewijze onbekend.

## DEEL D — VISUAL-SCRIPT TAXONOMY (VisualScriptRecord)
Scripts: relationeel vertrouwen, wederkerigheid, humor, status, challenge, groepsacceptatie, nieuwsgierigheid, impulsiviteit, bewijs van deelname, sociale performance, relationele verwachting, onbekend.
Structuur: { PrimaryScript, SecondaryScripts, ScriptIndicators, ScriptPhase, ReportedBy, Confidence }

## DEEL E — NORMALIZATION-CONTEXT (NormalizationContextRecord)
- Groepsframing: normaal, gebruikelijk, verwacht, grappig, speels, experimenteel, statusverhogend, riskant maar gebruikelijk, privé maar geaccepteerd, uitzonderlijk, ongewenst, omstreden, onbekend.
- Normbron: partner, vriendengroep, klas/schoolgenoten, feestgroep, sportteam, online community, platformcultuur, bredere jeugdcultuur, onbekend.
- Normmechanisme: voorbeeldgedrag, herhaald voorkomen, humor, complimenten, reacties/likes, statusbeloning, plagen, expliciete verwachting, impliciete verwachting, challengeformat, uitsluitingsdreiging, onbekend.
- Normen: DescriptiveNorm (wat jongeren denken dat anderen doen) vs InjunctiveNorm (wat jongeren denken dat anderen goedkeuren).

## DEEL F — DEVICE-MEDIATED AFFORDANCES (DeviceAffordanceRecord)
- Apparaat: mobiele telefoon, webcam, laptopcamera, tablet, externe camera, gedeeld apparaat, tweede opnameapparaat, onbekend.
- Platformtype: privéchat, groepschat, verdwijnberichtendienst, sociale media, story, videochat, groepsvideo, livestream, cloudopslag, onbekend.
- Opname-affordances: directe camera-opname, screenshot, schermopname, opname tweede apparaat, automatische opslag/archivering, lokale opslag, cloudback-up, opname door kijker, onbekend.
- Verspreidingsaffordances: 1-op-1 verzenden, doorsturen met weinig handelingen, groepschat delen, story plaatsen, openbaar uploaden, downloaden en heruploaden, platformoverschrijdend delen, sessielink delen, deelnemers toevoegen, onbekend.
- Tijdelijkheidsaffordances: 1-malig bekijken, verdwijnbericht, tijdelijke story, automatische verwijdering, screenshotmelding (aan/uit), schermopname mogelijk, opslag tweede apparaat mogelijk, cloud/cacheherstel mogelijk, onbekend.

## DEEL G — MEDIA-LIFECYCLE (MediaLifecycleRecord)
Lifecycle: capture -> storage -> first-share -> re-share -> persistence
- Capture: geen opname, bewuste zelfopname, bewuste opname door ander, gezamenlijke opname, opname door derde, screenshot, schermopname, opname tweede apparaat, automatische opname, opname zonder medeweten, onbekend.
- Storage: niet opgeslagen, lokaal opgeslagen, meerdere apparaten, tijdelijk opgeslagen, automatisch opgeslagen, cloudopslag, app-cache, direct verwijderd, verwijdering niet verifieerbaar, onbekend.
- First-share: niet gedeeld, getoond op hetzelfde apparaat, 1 ontvanger, partner, vriend, kleine besloten groep, groepschat, tijdelijk bericht, livestreampubliek, openbaar, onbekend.
- Re-share: niet verder gedeeld, met instemming verder gedeeld, zonder bekende instemming verder gedeeld, gekopieerd, screenshot, schermopname, naar andere groep verplaatst, platformoverschrijdend gedeeld, openbaar herplaatst, omvang onbekend.
- Persistence: niet bewaard, tijdelijk beschikbaar, lokaal bewaard, cloudkopie, meerdere kopieën, langdurig beschikbaar, publiek beschikbaar, vermoedelijk verwijderd, onbekend.
- Perceived ephemerality vs Actual persistence afzonderlijk gecodeerd.

## DEEL H — TRAJECTORY-MODEL (TrajectoryRecord)
Keten: trigger -> participation -> capture -> storage -> first-share -> re-share -> discovery -> response -> impact/recovery.
- Trigger: zelfstandig initiatief, wederzijds initiatief, direct verzoek, herhaald verzoek, relationele verwachting, groepsspel, dare/challenge, humor, nieuwsgierigheid, groepsnorm, sociale erkenning, feestcontext, alcohol/middelencontext, dreiging, onbekend.
- Participation: zelfstandig geïnitieerd, vrijwillig na verzoek, wederzijds afgesproken, impulsief, na sociale beïnvloeding, na herhaald aandringen, onder groepsdruk, onder relationele druk, onder dreiging, ambivalent, onbekend.
- Discovery: zelf teruggezien, melding partner/vriend, ontdekking groepschat/schoolnetwerk, ouder/verzorger ontdekt, platformmelding, hulpverlener, institutionele ontdekking, publieke ontdekking, onbekend.
- Response: geen actie, lachen, bagatelliseren, onderling bespreken, verzoek om verwijdering, blokkeren, groep verlaten, platformmelding, steun zoeken, gesprek vertrouwde persoon, schoolreactie, institutionele reactie, ontkenning, schuldtoewijzing, herstelpoging, onbekend.
- Impact: geen negatieve impact gerapporteerd, spijt, schaamte, onzekerheid, verlies van vertrouwen, relationeel conflict, pesten, uitsluiting, reputatie-effect, aanhoudende verspreiding, sociale terugtrekking, schoolproblemen, emotionele belasting, onbekend.
- Recovery: materiaal verwijderd, verspreiding beperkt, sociale steun, relatie hersteld, platforminterventie, school/hulpverleningssteun, veranderde privacypraktijken, geen herstel vastgesteld, onbekend.

## DEEL I — VISIBILITY-INTENT MISMATCH (VisibilityIntentMismatchRecord)
Typen: audience mismatch, temporality mismatch, purpose mismatch, context mismatch, identifiability mismatch, no mismatch established, unknown.
Omvang: geen aangetoonde mismatch, beperkt, substantieel, zeer groot, onbekend.

## DEEL J — INSTEMMING PER HANDELING (ConsentByActionRecord / InstemmingPerHandeling)
Fasen afzonderlijk coderen: deelname, opname, opslag, first-share, re-share, blijvende beschikbaarheid.
Waarden: expliciet, impliciet, ambivalent, onder druk, verondersteld, niet vastgesteld, geaccepteerd, niet verwacht, onbekend.

## DEEL K — CONTROLEVERLIES (ControlLossRecord)
FirstLossPoint: geen controleverlies vastgesteld, bij capture, bij automatische opslag, bij first-share, bij screenshot/schermopname, bij re-share, bij platformoverschrijdende verspreiding, bij publieke plaatsing, onbekend.

## DEEL L — MISSINGNESS-MAP (MissingnessMap)
Statuswaarden per variabele: gemeten, gerapporteerd, afgeleid, niet gemeten, niet gerapporteerd, tegenstrijdig, niet van toepassing.
STRIKTE REGEL: Geen stilzwijgende defaults (toestemming onbekend != vrijwillig; druk niet genoemd != geen druk; alcohol niet genoemd != nuchter; re-share niet genoemd != niet doorgestuurd; schade niet genoemd != geen schade).

## DEEL M — BEWIJSPROFIEL (EvidenceProfile)
Bronsoorten: representatieve survey, niet-representatieve survey, longitudinaal onderzoek, interviews, focusgroepen, etnografisch onderzoek, platformanalyse, contentanalyse, school/hulpverleningsdata, incidentrapport, mediabron, onbekend.

## DEEL N — FREQUENTIE EN VERGELIJKING
Content-frequency denominator ALTIJD verplicht bij percentages.
Behavioural granularity ladder: Niveau 0 (brede seksuele content) t/m Niveau 4 (volledig script, camerafunctie en publiek) en Niveau 5 (volledige lifecycle).
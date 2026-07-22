# MASTER CODEBOOK — Geïntegreerd Gedragsmatig Codeboek (Domein A t/m P)

Dit codeboek definieert het volledige analytische kader voor het classificeren, structureren en analyseren van visuele interacties en beeldmateriaal bij jongeren (15–18 jaar). Alle velden zijn neutraal, niet-juridisch en niet-moraliserend geformuleerd.

---

## 1. POPULATIONPROFILE (Domein A)

| Veld | Toegestane waarden |
|---|---|
| `Age` | 15 \| 16 \| 17 \| 18 |
| `AgeCohort` | "15 jaar" \| "16-17 jaar" \| "18 jaar" \| "12-25 jaar (breed)" |
| `Gender` | "M" \| "V" \| "NB" \| "ONBEKEND" |
| `SocialPosition` | "leerling" \| "student" \| "werkend" \| "anders" \| "ONBEKEND" |
| `Region` | "stedelijk" \| "platteland" \| "ONBEKEND" |
| `SampleType` | "representatief" \| "kwalitatief" \| "incident" \| "onbekend" |
| `PopulationBasis` | "leeftijdsgebaseerd" \| "schoolgebaseerd" \| "platformgebaseerd" \| "hulpverlening" \| "onbekend" |

---

## 2. CONTEXTVECTOR (Domein B)

| Veld | Toegestane waarden |
|---|---|
| `EventLocation` | "slaapkamer of andere privéruimte" \| "woning van vriend" \| "feestlocatie" \| "openbare ruimte" \| "schoolterrein" \| "digitale ruimte" \| "ONBEKEND" |
| `NetworkLocation` | "vaste relatie (1-op-1)" \| "vriendengroep" \| "groepschat (klas/jaarlaag)" \| "sociale media" \| "schoolnetwerk" \| "publiek platform" \| "ONBEKEND" |
| `HarmLocation` | "geen gerapporteerde schade" \| "klas/school" \| "lokaal sociaal netwerk" \| "sociale media" \| "hulpverlening" \| "politie & justitie" \| "gezin" \| "ONBEKEND" |
| `TimeContext` | Object met: `DayPart` ("ochtend"\|"middag"\|"avond"\|"nacht"), `WeekContext` ("schooldag"\|"weekend"\|"vakantie"), `Situation`, `Duration`, `Repetition` |
| `SocialRelation` | "partner (vaste relatie)" \| "ex-partner" \| "vriend" \| "vriendengroep" \| "klasgenoot" \| "online bekende" \| "ONBEKEND" |
| `GroupSize` | "1-op-1" \| "kleine groep (2-5)" \| "middelgrote groep (5-15)" \| "grote groep (15+)" \| "ONBEKEND" |

---

## 3. BEHAVIOURALCONTENTRECORD (Domein C)

| Veld | Toegestane waarden |
|---|---|
| `VisibilityLevel` | "volledig gekleed" \| "gedeeltelijk ontkleed" \| "bovenlichaam gedeeltelijk" \| "naaktheid" \| "onduidelijk" \| "NIET GERAPPORTEERD" |
| `BehaviourClass` | "poseren voor camera" \| "kleding verwijderen" \| "lichaam tonen" \| "intieme houding of gebaar" \| "zelfgerichte seksuele handeling (breed)" \| "seksuele interactie (breed)" \| "uitvoering opdracht/challenge" \| "gedrag onbekend" |
| `ParticipantConfiguration` | "solo" \| "solo met kijker" \| "twee personen" \| "meerdere personen" \| "één zichtbaar + anderen buiten beeld" \| "ONBEKEND" |
| `LiveOrRecorded` | "uitsluitend live" \| "live + opname" \| "vooraf opgenomen" \| "screenshot" \| "schermopname" \| "ONBEKEND" |
| `InitiationMode` | "zelf geïnitieerd" \| "wederzijds" \| "na direct verzoek" \| "na herhaald verzoek" \| "dare/challenge" \| "groepsdruk" \| "ONBEKEND" |
| `CameraOrientation` | "zelfopname" \| "door andere deelnemer" \| "door derde" \| "webcam" \| "schermopname" \| "ONBEKEND" |
| `RecorderRelation` | "zelf opgenomen" \| "door deelnemer" \| "door derde" \| "op afstand opgenomen" \| "ONBEKEND" |
| `SocialFunction` | "relationele intimiteit" \| "nieuwsgierigheid" \| "humor/speelsheid" \| "challenge/dare" \| "groepsacceptatie" \| "status/erkenning" \| "bewijs van deelname" \| "ONBEKEND" |
| `IntendedAudience` | "alleen maker" \| "één ontvanger" \| "partner" \| "vriend" \| "beperkte groep" \| "groepschat" \| "publiek" \| "ONBEKEND" |
| `ActualAudience` | "gelijk aan bedoeld" \| "beperkt uitgebreid" \| "schoolnetwerk" \| "meerdere groepen" \| "openbaar platform" \| "ONBEKEND" |

---

## 4. VISUALSCRIPTRECORD (Domein D)

| Veld | Toegestane waarden |
|---|---|
| `PrimaryScript` | "relationeel vertrouwen" \| "humor/speelsheid" \| "status/erkenning" \| "challenge/dare" \| "groepsacceptatie" \| "nieuwsgierigheid/experiment" \| "impulsiviteit" \| "bewijs van deelname" \| "ONBEKEND" |
| `SecondaryScripts` | Array van bovenstaande waarden |
| `ScriptPhase` | "trigger" \| "participation" \| "capture" \| "first-share" \| "re-share" \| "discovery" |
| `ReportedBy` | "deelnemer (maker)" \| "deelnemer (ontvanger)" \| "derde" \| "onderzoeker" \| "ONBEKEND" |
| `Confidence` | "hoog" \| "middel" \| "laag" |

---

## 5. NORMALIZATIONCONTEXTRECORD (Domein E)

| Veld | Toegestane waarden |
|---|---|
| `SocialGroup` | "vriendengroep" \| "klas" \| "school" \| "online community" \| "sportvereniging" \| "ONBEKEND" |
| `NormalizationFrame` | "privé geaccepteerd" \| "genormaliseerd binnen relatie" \| "genormaliseerd in groep" \| "afgekeurd" \| "ONBEKEND" |
| `DescriptiveNorm` | Omschrijving van gepercipieerde norm |
| `InjunctiveNorm` | Omschrijving van wat goedkeuring krijgt |
| `PerceivedPrevalence` | Geschatte prevalentie (percentage of "hoog"/"laag") |
| `MeasuredPrevalence` | Werkelijk gemeten prevalentie |
| `BoundaryConditions` | Grenzen van acceptatie |
| `Dissent` | "stille weerstand" \| "expliciete afwijzing" \| "geen" \| "ONBEKEND" |

---

## 6. DEVICEAFFORDANCERECORD (Domein F)

| Veld | Toegestane waarden |
|---|---|
| `Device` | "mobiele telefoon (GSM)" \| "laptop" \| "webcam" \| "tablet" \| "camera" \| "ONBEKEND" |
| `PlatformType` | "verdwijnberichtendienst" \| "berichtenapp" \| "sociale media" \| "videochat" \| "groepschat" \| "ONBEKEND" |
| `CaptureAffordances` | Array: "directe camera-opname" \| "screenshot" \| "schermopname" \| "tweede apparaat" \| "automatische opslag" |
| `EphemeralityAffordances` | Array: "verdwijnbericht" \| "éénmalig bekijken" \| "geen indicator" \| "screenshot-melding" |
| `DistributionFriction` | "laag" \| "middel" \| "hoog" |

---

## 7. MEDIALIFECYCLERECORD (Domein G)

| Veld | Toegestane waarden |
|---|---|
| `Capture` | "bewuste zelfopname" \| "bewuste opname door ander" \| "schermopname" \| "screenshot" \| "tweede apparaat" \| "automatisch" \| "ONBEKEND" |
| `Storage` | "tijdelijk (app)" \| "lokaal toestel" \| "cloud" \| "meerdere apparaten" \| "ONBEKEND" |
| `FirstShare` | "partner (1-op-1)" \| "vriend" \| "beperkte groep" \| "groepschat" \| "ONBEKEND" |
| `ReShare` | "geen" \| "met toestemming" \| "zonder toestemming" \| "via screenshot" \| "ONBEKEND" |
| `PerceivedEphemerality` | "verdwijnend verondersteld" \| "tijdelijk bedoeld" \| "permanent bedoeld" \| "ONBEKEND" |
| `ActualPersistence` | "lokaal opgeslagen" \| "cloud-back-up" \| "screenshot bij derden" \| "publiek beschikbaar" \| "ONBEKEND" |

---

## 8. TRAJECTORYRECORD (Domein H)

| Fase | Toegestane waarden |
|---|---|
| `Trigger` | "direct verzoek" \| "wederzijds initiatief" \| "dare/challenge" \| "relationeel verzoek" \| "humor/nieuwsgierigheid" \| "herhaald aandringen" \| "dreiging/chantage" \| "ONBEKEND" |
| `Participation` | "zelfstandig geïnitieerd" \| "vrijwillig na verzoek" \| "impulsief" \| "onder sociale beïnvloeding" \| "onder groepsdruk" \| "dwang" \| "ONBEKEND" |
| `Capture` | Zie MediaLifecycle.Capture |
| `Storage` | Zie MediaLifecycle.Storage |
| `FirstShare` | Zie MediaLifecycle.FirstShare |
| `ReShare` | Zie MediaLifecycle.ReShare |
| `Discovery` | "deelnemer ziet terug" \| "melding door vriend" \| "confrontatie op school" \| "ouder ontdekt" \| "politie/platform" \| "ONBEKEND" |
| `Response` | "geen actie" \| "lachen/bagatelliseren" \| "verwijderingsverzoek" \| "blokkeren" \| "melding aan school/politie" \| "hulp zoeken" \| "ONBEKEND" |
| `Impact` | "geen schade gerapporteerd" \| "spijt" \| "schaamte" \| "pesten/uitsluiting" \| "reputatieschade" \| "chantage" \| "psychische gevolgen" \| "ONBEKEND" |
| `Recovery` | "geen interventie" \| "materiaal verwijderd" \| "sociale steun" \| "schoolinterventie" \| "hulpverlening" \| "juridisch" \| "ONBEKEND" |

---

## 9. VISIBILITYINTENTMISMATCHRECORD (Domein I)

| Veld | Toegestane waarden |
|---|---|
| `MismatchTypes` | Array: "audience mismatch" \| "temporality mismatch" \| "purpose mismatch" \| "context mismatch" \| "identity mismatch" |
| `MismatchMagnitude` | "geen" \| "beperkt" \| "substantieel" \| "totaal" |
| `IntendedPurpose` | Zie `SocialFunction` |
| `ActualUse` | "relationele communicatie" \| "humoristische performance" \| "statusmateriaal" \| "chantage" \| "vergelding" \| "ONBEKEND" |
| `Identifiability` | "volledig herkenbaar" \| "deels herkenbaar" \| "niet herkenbaar" \| "ONBEKEND" |

---

## 10. CONSENTBYACTIONRECORD (Domein J)

| Veld | Toegestane waarden |
|---|---|
| `ParticipationConsent` | "expliciet" \| "verondersteld" \| "onder druk" \| "niet vastgesteld" \| "NIET VAN TOEPASSING" |
| `CaptureConsent` | "expliciet" \| "verondersteld" \| "zonder medeweten" \| "niet vastgesteld" |
| `StorageConsent` | "expliciet" \| "verondersteld" \| "niet verwacht" \| "niet vastgesteld" |
| `FirstShareConsent` | "expliciet" \| "verondersteld" \| "niet vastgesteld" |
| `ReShareConsent` | "expliciet" \| "verondersteld" \| "niet vastgesteld" \| "expliciet geweigerd" |

---

## 11. CONTROLLOSSRECORD (Domein K)

| Veld | Toegestane waarden |
|---|---|
| `FirstLossPoint` | "bij opname" \| "bij opslag" \| "bij first-share" \| "bij screenshot" \| "bij re-share" \| "ONBEKEND" |
| `LossDomains` | Array: "aantal kopieën" \| "ontvangers" \| "verdere verspreiding" \| "context" |
| `Reversibility` | "reversibel" \| "irreversibel" \| "deels reversibel" \| "ONBEKEND" |
| `ParticipantAwareness` | "bekend op moment" \| "ontdekt achteraf" \| "nog steeds onbekend" \| "ONBEKEND" |

---

## 12. RESPONSEANDRECOVERYRECORD (Domein L)

| Veld | Toegestane waarden |
|---|---|
| `ResponseActions` | Array: "verwijderingsverzoek" \| "blokkeren" \| "melding school" \| "melding politie" \| "gesprek vertrouwenspersoon" \| "hulp gezocht" \| "geen actie" |
| `ImpactObserved` | Array: "spijt" \| "schaamte" \| "pesten" \| "reputatie-effect" \| "relationeel conflict" \| "psychische klachten" \| "geen impact" |
| `RecoverySupport` | Array: "sociale steun" \| "schoolinterventie" \| "hulpverlening" \| "juridisch" \| "geen" |
| `Status` | "geen interventie nodig" \| "actief herstel" \| "afgerond" \| "onbekend" |

---

## 13. DELTAFIELDRECORD (Domein M)

| Veld | Toegestane waarden |
|---|---|
| `BehaviourToImageConversionPoint` | "opname vanaf begin" \| "opname halverwege" \| "achteraf voorgesteld" \| "bewijs" \| "automatisch" \| "ONBEKEND" |
| `PromptSourceMap` | "deelnemer zelf" \| "partner" \| "vriend" \| "groep" \| "groepschat" \| "online kijker" \| "challenge" \| "ONBEKEND" |
| `ContentEscalationPath` | "poseren → kleding verwijderen → lichaam tonen → breder" |
| `CameraPresenceEffect` | "geen effect" \| "meer cameragericht" \| "bewijsgedreven" \| "publiekgedreven" \| "ONBEKEND" |
| `AudienceFeedbackLoop` | "verzoeken" \| "aanmoediging" \| "complimenten" \| "groepsdruk" \| "afwijzing" \| "ONBEKEND" |
| `SessionBoundary` | "één korte interactie" \| "één langere sessie" \| "meerdere sessies" \| "terugkerend" \| "ONBEKEND" |
| `CountingUnitProtocol` | "personen" \| "gebeurtenissen" \| "sessies" \| "beelden" \| "berichten" \| "meldingen" |
| `BehaviouralStoppingPoint` | "deelnemer wil niet verder" \| "verzoek afgewezen" \| "technische onderbreking" \| "spijt/twijfel" \| "ONBEKEND" |

---

## 14. MISSINGNESSMAP (Domein N)

Voor elk variabel veld in het IncidentRecord wordt de informatiestatus gecodeerd:

### Statuswaarden
- `GEMETEN`: Rechtstreeks onderzocht/bevraagd in bron
- `GERAPPORTEERD`: Expliciet vermeld, maar geen formeel meetinstrument
- `AFGELEID`: Logisch afgeleid (verplicht met `InferenceReason` en `Confidence`)
- `NIET GEMETEN`: Niet opgenomen in onderzoeksopzet
- `NIET GERAPPORTEERD`: Mogelijk gemeten, maar niet gepubliceerd
- `TEGENSTRIJDIG`: Incompatibele informatie uit bronnen
- `NIET VAN TOEPASSING`: Variabele niet relevant voor casus

### Geen stilzwijgende defaults
1. Toestemming onbekend ≠ Vrijwillig
2. Dwang niet genoemd ≠ Geen dwang
3. Alcohol niet genoemd ≠ Nuchter
4. Locatie niet genoemd ≠ Thuis
5. Re-share niet genoemd ≠ Niet doorgestuurd
6. Verwijdering gemeld ≠ Definitief verdwenen
7. Lachen/bagatelliseren genoemd ≠ Geen schade

### Syntax
```json
{
  "VariableName": {
    "Status": "GEMETEN | GERAPPORTEERD | AFGELEID | NIET GEMETEN | NIET GERAPPORTEERD | TEGENSTRIJDIG | NIET VAN TOEPASSING",
    "ReportedValue": "waarde of null",
    "EvidenceLocation": "bronverwijzing of null",
    "InferenceReason": "reden bij AFGELEID of null",
    "Confidence": "hoog | middel | laag | niet van toepassing"
  }
}
```

---

## 15. EVIDENCEPROFILE (Domein O)

| Veld | Toegestane waarden |
|---|---|
| `SourceType` | "representatieve survey" \| "kwalitatief interview" \| "incidentmelding" \| "politiedata" \| "hulpverleningsdata" \| "mediabericht" \| "onbekend" |
| `EvidenceStatus` | "rechtstreeks gemeten" \| "zelfgerapporteerd" \| "afgeleid uit bron" \| "onbekend" |
| `SourceVisibilityBias` | "zelfrapportage" \| "schoolinterventie" \| "politie/justitie" \| "hulpverlening" \| "media" \| "onbekend" |
| `GranularityLevel` | 0 \| 1 \| 2 \| 3 \| 4 |
| `ContentFrequencyDenominator` | "alle jongeren" \| "jongeren die ooit maakten" \| "jongeren die ooit ontvingen" \| "jongeren die doorstuurden" \| "incidentmeldingen" |

---

## 16. NON-EVENT BASELINE (Domein P — dwarsdoorsnijdend)

Verplichte registratie voor alle casussen: geef aan of er sprake is van een Non-Event Baseline (geen escalatie, geen schade, geen ongeautoriseerde verspreiding).

```json
{
  "NonEventBaseline": true | false,
  "BaselineType": "besloten gebleven" | "consensueel" | "geen schade" | "niet van toepassing"
}
```

---

## VOLLEDIGE INCIDENTRECORD-SYNTAX

```json
{
  "incident_id": "string",
  "timestamp": "ISO 8601",
  "PopulationProfile": { },
  "ContextVector": { },
  "BehaviouralContentRecord": { },
  "VisualScriptRecord": { },
  "NormalizationContextRecord": { },
  "DeviceAffordanceRecord": { },
  "MediaLifecycleRecord": { },
  "TrajectoryRecord": { },
  "VisibilityIntentMismatchRecord": { },
  "ConsentByActionRecord": { },
  "ControlLossRecord": { },
  "ResponseAndRecoveryRecord": { },
  "DeltaFieldRecord": { },
  "MissingnessMap": { },
  "EvidenceProfile": { }
}
```

# DELTA INSIGHTS — Gedragsladders, Frequentienoemers & Escalatiescores

Operationele definities van de 20 verplichte Delta-inzichten voor analyse van visuele interacties bij jongeren (15–18 jaar).

---

## 1. BEHAVIOURAL GRANULARITY LADDER (Analyse-niveau)

Voorkomt schijnprecisie: bronnen worden gecodeerd op het hoogste detailniveau dat ze ondersteunen.

| Niveau | Beschrijving |
|---|---|
| **Niveau 0** | Containerbegrippen ("sexting", "seksuele content") |
| **Niveau 1** | Kleding- en naaktheidsniveau |
| **Niveau 2** | Gedragsklasse (poseren, tonen, ontkleden, interactie) |
| **Niveau 3** | Interactiestructuur + gedragsklasse |
| **Niveau 4** | Gedragsklasse + sociaal script + camerarelatie |

**Regel:** Vergelijk studies uitsluitend op hetzelfde of lager niveau.

---

## 2. CONTENT-FREQUENCY DENOMINATOR (Noemer-standaardisatie)

Frequenties worden alleen gerapporteerd met expliciete noemer:

| Code | Noemer |
|---|---|
| `DENOM_01` | Alle jongeren in populatiesample |
| `DENOM_02` | Jongeren die ooit beelden maakten/verstuurden |
| `DENOM_03` | Jongeren die ooit intieme beelden ontvingen |
| `DENOM_04` | Jongeren die ooit beelden doorstuurden (re-share) |
| `DENOM_05` | Steekproef van gerapporteerde incidenten |

---

## 3. CAPTURE-DEPENDENCY FIELD (Media-afhankelijkheid)

| Waarde | Betekenis |
|---|---|
| `Pre-existing` | Gedrag zou ook zonder camera hebben plaatsgevonden |
| `Camera-induced` | Specifiek voor en vanwege de camera uitgevoerd |
| `Proof-driven` | Uitsluitend als bewijsstuk voor challenge/verzoek |
| `Audience-driven` | Aangewakkerd door live publiek of kijkersreacties |

---

## 4. CONTENT-TO-CIRCULATION TRANSFORMATION (Betekenisverschuiving)

Vastleggen hoe de sociale betekenis van hetzelfde beeld transformeert:

```
Privé-communicatie → Groepsgrap → Statusmateriaal → Publiek/Institutioneel Incident
```

---

## 5. VIEWER-PARTICIPATION LAYER (Kijkersrol)

Codeert actieve rol van ontvangers/kijkers in live- en groepscontext:

- Passief kijken
- Verzoeken doen
- Live aanmoedigen/opjutten
- Beloningen geven
- Screenshots/schermopnames maken
- Actief doorsturen
- Weigeren/ingrijpen/beschermen

---

## 6. REQUEST-TO-ACTION DISTANCE (Tijds- en Drukafstand)

| Waarde | Betekenis |
|---|---|
| Onmiddellijk/Impulsief | Binnen seconden/minuten |
| Korte aarzeling | Na milde twijfel of pauze |
| Na herhaald verzoek | Pas na meervoudig vragen |
| Na groepsdruk/beloning | Gestuurd door live reacties |
| Gepland | Op later afgesproken moment |

---

## 7. VISIBILITY ESCALATION SCORE (Escalatie-ladder)

Codeert kwantitatieve uitbreiding van zichtbaarheid:

| Level | Bereik |
|---|---|
| Level 0 | Alleen maker (geen verzending) |
| Level 1 | 1-op-1 ontvanger (partner/vriend) |
| Level 2 | Kleine besloten groep |
| Level 3 | School-/klasnetwerk |
| Level 4 | Openbaar platform/publiek |

---

## 8. CONTENT-SOURCE BIAS (Bron-vertekening)

| Bron | Vertekeningsrichting |
|---|---|
| Surveys | Oververtegenwoordigen lichte vormen, consensuele selfies |
| Interviews | Hoge diepgang, geen representatieve frequenties |
| Schoolbronnen | Zien alleen escalaties die leiden tot conflict op school |
| Hulpverlening/Justitie | Zien alleen zwaarste escalatietrajecten |

---

## 9. NON-EVENT BASELINE (Referentiekader zonder Escalatie)

Verplichte opname van casussen zonder escalatie, schade of ongeautoriseerde verspreiding:
- Beeldmateriaal bleef besloten
- Geen re-share opgetreden
- Geen emotionele of sociale schade gerapporteerd
- Deelnemers evalueren ervaring als neutraal of positief

**Regel:** Elk onderzoek moet minimaal 1 Non-Event Baseline bevatten om escalatie-bias te voorkomen.

---

## 10. SEQUENCE-PATTERN LIBRARY (Trajecten-bibliotheek)

### Patroon Alpha (Besloten relatiedynamiek)
```
Relationeel vertrouwen → Privé-opname (GSM) → First-share partner → Geen re-share → Geen schade
```

### Patroon Beta (Groeps/status-escalatie)
```
Groepsgrap/Dare → Cameragerichte uitvoering → First-share groepschat → Ongeautoriseerde re-share → Schoolnetwerk
```

### Patroon Gamma (Live webcamescalatie)
```
Live challenge/Exploratie → Webcamperformance → Schermopname achtergrond → Platformoverschrijdend → Hulpverlening/Justitie
```

---

## 11. BEHAVIOUR-TO-IMAGE CONVERSION POINT (Gedrag-naar-Beeld-omzetpunt)

Codeert op welk moment in de interactie de beslissing valt om van gedrag naar vastgelegde beelda productie over te gaan:

| Waarde | Betekenis |
|---|---|
| `Opname vanaf begin` | Deelnemer start met opname en gedrag volgt |
| `Opname halverwege` | Gedrag begint, camera wordt later toegevoegd |
| `Achteraf voorgesteld` | Er wordt pas na het gedrag besloten iets vast te leggen |
| `Bewijs` | Vastlegging als bewijsstuk voor challenge/verzoek |
| `Automatisch` | Systeem legt vast zonder menselijke tussenkomst |
| `ONBEKEND` | Onvoldoende informatie |

---

## 12. PROMPT-SOURCE MAP (Bron van het verzoek)

Brengt de bron van het verzoek tot beeldproductie in kaart:

| Waarde | Betekenis |
|---|---|
| `Deelnemer zelf` | Eigen initiatief, geen externe aanleiding |
| `Partner` | Verzoek van vaste relatiepartner |
| `Vriend` | Verzoek van een individuele vriend |
| `Groep` | Verzoek van een vriendengroep |
| `Groepschat` | Verzoek via digitale groepschat |
| `Online kijker` | Verzoek van een anonieme online kijker |
| `Challenge` | Verzoek als onderdeel van een online challenge/dare |
| `ONBEKEND` | Onvoldoende informatie |

---

## 13. CONTENT ESCALATION PATH (Escalatiepad van inhoud)

Vast pad waarlangs de inhoud van beeldmateriaal kan escaleren tijdens een sessie:

```
Poseren → Kleding verwijderen → Lichaam tonen → Seksuele handeling
```

Niet elke sessie doorloopt alle fasen. Codeer waar de sessie stopt.

---

## 14. CAMERA-PRESENCE EFFECT (Camera-aanwezigheidseffect)

Codeert hoe de aanwezigheid van een camera het gedrag beïnvloedt:

| Waarde | Betekenis |
|---|---|
| `Geen effect` | Gedrag is natuurlijk, camera verandert niets |
| `Meer cameragericht` | Deelnemer richt gedrag naar de camera |
| `Bewijsgedreven` | Handelingen worden herhaald/geënsceneerd voor bewijs |
| `Publiekgedreven` | Gedrag wordt opgevoerd voor (verondersteld) publiek |
| `ONBEKEND` | Onvoldoende informatie |

---

## 15. AUDIENCE FEEDBACK LOOP (Publieksfeedback-lus)

Codeert wat voor feedback een live of asynchroon publiek geeft tijdens een sessie:

| Waarde | Betekenis |
|---|---|
| `Verzoeken` | Publiek vraagt om specifieke handelingen |
| `Aanmoediging` | Publiek moedigt aan (positieve bekrachtiging) |
| `Complimenten` | Positieve feedback op uiterlijk/gedrag |
| `Groepsdruk` | Publiek oefent druk uit om door te gaan |
| `Afwijzing` | Negatieve reacties |
| `ONBEKEND` | Onvoldoende informatie |

---

## 16. SESSION-BOUNDARY FIELD (Sessiegrens)

Codeert de temporele grenzen van een visuele interactie:

| Waarde | Betekenis |
|---|---|
| `Eén korte interactie` | Enkele seconden tot minuten, eenmalig |
| `Eén langere sessie` | Aaneengesloten sessie van 10+ minuten |
| `Meerdere sessies` | Meerdere aparte sessies, zelfde deelnemers |
| `Terugkerend` | Structureel terugkerend patroon |
| `ONBEKEND` | Onvoldoende informatie |

---

## 17. IMAGE-SET STRUCTURE (Beeldenset-structuur)

Codeert of het beeldmateriaal uit één of meerdere beelden bestaat en wat de onderlinge relatie is:

| Waarde | Betekenis |
|---|---|
| `Enkel beeld` | Eén enkel stilstaand beeld |
| `Reeks opeenvolgend` | Meerdere beelden in chronologische volgorde |
| `Selectie` | Keuze uit meerdere gemaakte beelden |
| `Video-opname` | Doorlopende video |
| `Burst/Serie` | Snel opeenvolgende opnames |
| `ONBEKEND` | Onvoldoende informatie |

---

## 18. COUNTING-UNIT PROTOCOL (Tel-eenheid-protocol)

Standaardiseert hoe frequenties worden geteld in onderzoek en analyse:

| Waarde | Toepassing |
|---|---|
| `Personen` | Aantal unieke deelnemers dat beeldmateriaal maakte/ontving |
| `Gebeurtenissen` | Aantal aparte incidenten/verzoeken |
| `Sessies` | Aantal aparte interactiemomenten |
| `Beelden` | Aantal unieke beeldbestanden |
| `Berichten` | Aantal verzonden berichten (incl. beeld) |
| `Meldingen` | Aantal gerapporteerde incidenten bij instanties |

**Regel:** Specificeer altijd de gebruikte teleenheid bij rapportage van frequenties.

---

## 19. BEHAVIOURAL STOPPING POINT (Gedragsstop-punt)

Codeert waarom een visuele interactie stopt of waarom een deelnemer niet verdergaat:

| Waarde | Betekenis |
|---|---|
| `Deelnemer wil niet verder` | Eigen grens bereikt |
| `Verzoek afgewezen` | Verzoek tot verdere handeling geweigerd |
| `Technische onderbreking` | Apparaat/platform onderbreekt |
| `Spijt/twijfel` | Terugtrekking na twijfel of spijt |
| `Extern ingrijpen` | Ouder/school/derde grijpt in |
| `ONBEKEND` | Onvoldoende informatie |

---

## 20. CROSS-SOURCE TRANSLATION TABLE (Empirische term → Codeboek-vertaling)

Empirische onderzoeks-termen neutraal koppelen aan Codeboek-categorieën (Granulariteitsniveau 0 t/m 4).

### Niveau 0 — Containerbegrippen

| Empirische term | Neutrale Codeboek-vertaling |
|---|---|
| "Sexting" | Containerterm; specificeer gedragsklasse + visibility level |
| "Seksuele content" | Containerterm; specificeer gedragsklasse |
| "Naaktfoto" | VisibilityLevel = naaktheid + BehaviourClass specificeren |
| "Intieme beelden" | VisibilityLevel ≥ gedeeltelijk ontkleed |
| "Ongepaste foto's" | **NIET GEBRUIKEN** — moraliserende lading; vervang door VisibilityLevel + BehaviourClass |
| "Explliciet materiaal" | **NIET GEBRUIKEN** — juridische connotatie; vervang door descriptieve gedragsklasse |
| "Pornografisch" | **NIET GEBRUIKEN** — juridisch geladen; vervang door BehaviourClass + LiveOrRecorded |

### Niveau 1 — Kleding- en naaktheidsniveau

| Empirische term | Neutrale Codeboek-vertaling |
|---|---|
| "Fully dressed" | VisibilityLevel = volledig gekleed |
| "Half naked" | VisibilityLevel = gedeeltelijk ontkleed |
| "Topless" | VisibilityLevel = bovenlichaam gedeeltelijk |
| "Naked/nude" | VisibilityLevel = naaktheid |
| "Underwear photo" | VisibilityLevel = gedeeltelijk ontkleed |
| "Swimsuit" | VisibilityLevel = volledig gekleed (sociaal aanvaardbaar) |

### Niveau 2 — Gedragsklasse

| Empirische term | Neutrale Codeboek-vertaling |
|---|---|
| "Selfie" | CameraOrientation = zelfopname; specificeer VisibilityLevel |
| "Posing" | BehaviourClass = poseren voor camera |
| "Flashing" | BehaviourClass = lichaam tonen (kortdurend) |
| "Masturbation" | BehaviourClass = zelfgerichte seksuele handeling (breed) |
| "Sexual performance" | BehaviourClass = seksuele interactie (breed) |
| "Sexual act with partner" | BehaviourClass = seksuele interactie (breed) |
| "Dare execution" | InitiationMode = dare/challenge; BehaviourClass specifiek |
| "Strip tease" | BehaviourClass = kleding verwijderen |

### Niveau 3 — Interactiestructuur + gedragsklasse

| Empirische term | Neutrale Codeboek-vertaling |
|---|---|
| "Couple sexting" | ParticipantConfiguration = twee personen; BehaviourClass specificeren |
| "Group sexting" | ParticipantConfiguration = meerdere personen |
| "Live sexting" | LiveOrRecorded = uitsluitend live |
| "Snapchat sexting" | PlatformType = verdwijnberichtendienst; PerceivedEphemerality = verdwijnend verondersteld |
| "Screen recording" | Capture = schermopname |
| "Screenshotting" | Capture = screenshot; ReShare = zonder toestemming |
| "Webcam show" | CameraOrientation = webcam; initiatie = na verzoek/beloning |
| "Dick pic" | BehaviourClass = lichaam tonen (geslachtsdeel); VisibilityLevel = naaktheid |
| "Upskirting" | CameraOrientation = door derde; CaptureConsent = zonder medeweten |
| "Revenge porn" | **NIET GEBRUIKEN** — juridisch/moraliserend; vervang door re-share zonder toestemming + motief: vergelding |
| "Non-consensual sharing" | ReShare = zonder toestemming |

### Niveau 4 — Gedragsklasse + sociaal script + camerarelatie

| Empirische term | Neutrale Codeboek-vertaling |
|---|---|
| "Consensual intimate selfie" | InitiationMode = zelf geïnitieerd of wederzijds; CaptureConsent = expliciet; SocialFunction = relationele intimiteit |
| "Partner sharing" | SocialRelation = partner (vaste relatie); FirstShare = partner |
| "Dare-based group sharing" | InitiationMode = dare/challenge; NetworkLocation = vriendengroep; ScriptPhase = participation |
| "Coerced sharing" | InitiationMode = na herhaald verzoek of groepsdruk; Participation = onder sociale beïnvloeding |
| "Screenshot leak" | Capture = screenshot; ReShare = zonder toestemming; MismatchTypes = audience mismatch |
| "Trust violation" | MismatchTypes = purpose mismatch; ImpactObserved bevat relationeel conflict |
| "Mutual exchange" | InitiationMode = wederzijds; FirstShareConsent = expliciet; Geen schade |
| "Voyeuristic capture" | CaptureConsent = zonder medeweten; CameraOrientation = door derde |
| "Self-produced image" | CameraOrientation = zelfopname; RecorderRelation = zelf opgenomen |
| "Peer-produced image" | CameraOrientation = door andere deelnemer; RecorderRelation = door deelnemer |
| "Sextortion" | **NIET GEBRUIKEN** — juridisch; vervang door: dreiging/chantage als trigger + Impact = chantage + Participation = dwang |
| "CSAM/child sexual abuse material" | **NIET GEBRUIKEN** — juridisch en strafrechtelijk; vervang door BehaviourClass + VisibilityLevel + CaptureConsent + Participation |

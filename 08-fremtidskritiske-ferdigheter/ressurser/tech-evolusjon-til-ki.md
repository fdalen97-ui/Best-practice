# Fra PC til internett til KI — overføringer som faktisk gjelder

## Hva er dette

En lesning av tre teknologibølger — personlig datamaskin (1975–1995), internett (1993–2015) og KI (2022–?) — for å se hvilke mønstre som gjentar seg, hvilke som ikke gjør det, og hvor i kurven KI faktisk er nå. Ikke en historietime; et navigasjonsverktøy for å vurdere egne valg i RFP Studio, PFT-portefølje og AI-governance.

## Hvorfor for meg spesifikt

Tre grunner:

1. **Kalibrere hype**. Hver bølge har samme retoriske kurve («dette endrer alt» → skuffelse → faktisk endring). Å kjenne kurven gjør det lettere å skille signal fra støy *underveis*, ikke i ettertid.
2. **Posisjonere før loven kommer**. Internett gikk uregulert i 25 år før GDPR. KI får ikke samme nådetid. Den som leser kurven riktig posisjonerer seg før reguleringsbølgen, ikke etter.
3. **Vite hvor «VisiCalc-momentet» er**. Det er ett eller to grep i dette tiåret som tilsvarer regneark for PC eller søk for internett. RFP Studio kan være det for sitt domene. Det forutsetter at jeg ser etter riktig form.

## De tre bølgene — fasekartet

| Fase | PC (1975–1995) | Internett (1993–2015) | KI (2022–?) |
|---|---|---|---|
| **Forløper** | Mainframe, minicomputer (60–70-tall). Stordrift, sentralisert. | ARPANET, akademiske nett (70–80-tall). Lukket, ekspertdrevet. | Frontier labs, forskning (2017–2022). GPT-2/3, BERT. Lukket, ekspertdrevet. |
| **Hobbyfase** | Altair, Apple I, hjemmebrygget. Få brukere, høy teknisk terskel. | BBS, Usenet, gopher. Tekstbasert, små miljøer. | Playground, GPT-3 API (2020–22). Få brukere, prompting som folkekunst. |
| **Konsumentmoment** | IBM PC + Windows 3.1 (1990–92). Brød-og-smør-bruk i kontor. | Mosaic/Netscape (1994–95). Web åpner for «vanlige folk». | ChatGPT (nov 2022). 100M brukere på 2 måneder. |
| **Killer-app** | Regneark (VisiCalc/Lotus/Excel). Endret regnskap og finans. | Søk (Google, ~1998–2003) og e-handel (Amazon). | *Under definering.* Coding-assistenter er det som ligner mest, så langt. |
| **Plattformkrig** | DOS vs Mac vs OS/2. Wintel-konsolidering. | Netscape vs IE. Mobil: iOS vs Android. | OpenAI vs Anthropic vs Google vs open weights. Pågår nå. |
| **Distribusjonsskifte** | Sentralt → personlig (PC på hvert skrivebord). | Skrivebord → lomme (mobil, 2007+). | Sky → lokalt/embedded (on-prem, edge, on-device). Tidlig nå. |
| **Governance-bølge** | Antitrust (Microsoft 1998). Sent. | GDPR 2018, plattformregulering 2020+. Veldig sent. | EU AI Act 2024–26, sektorregulering. Tidligere enn de to forrige. |
| **Modning** | Embedded i alt (innbakt i bil, hvitevarer). | Embedded i alt (IoT, sensorer). | *For tidlig.* Forventning: embedded i alt 2030+. |

## Mønstre som gjentar seg

### 1. Kostnadskurven faller ~10× hvert 2.–3. år, deretter blir grenseflaten viktig

PC: pris per MIPS falt eksponensielt 1975–2000. Internett: pris per GB overført falt eksponensielt 1995–2015. KI: pris per million inferens-tokens har falt >100× fra 2022 til 2026.

Implikasjonen er den samme i alle tre: når kostnaden ikke er flaskehalsen lenger, blir *grensesnittet* og *integrasjonen* den nye flaskehalsen. Excel slo ikke fordi det var raskere enn Lotus, men fordi Windows-grensesnittet vant. Google slo ikke fordi det var billigere, men fordi grensesnittet var renere. KI-vinnere i 2027–28 vil ikke vinne på modellkvalitet alene — de vinner på integrasjon, agent-arkitektur, evals og brukerflyt.

For RFP Studio: ikke konkurrer på modell. Konkurrer på agent-mønster, evals og workflow-integrasjon.

### 2. Sentralisert → distribuert → embedded

Mainframe → PC → laptop → mobil → smartklokke.
Server → sky → edge → on-device.
Frontier API → mindre modeller → lokale modeller → on-device modeller.

Dette er ikke samme bevegelse fysisk, men samme bevegelse økonomisk: når enhetskostnaden faller nok, går teknologien fra delt ressurs til personlig ressurs til usynlig ressurs. KI er nå rundt overgangen «delt → personlig» (lokale modeller på laptop). «Personlig → usynlig» kommer mellom 2027 og 2030.

For PFT-portefølje: alt som krever cloud-API i dag og er kjernekritisk, må kunne kjøres lokalt om 24 måneder. Lag arkitekturen for det nå.

### 3. Killer-apps oppdages i fase 2, ikke fase 1

VisiCalc kom 4 år etter Apple II. Google kom 5 år etter Mosaic. iPhone-app-økonomien kom 1 år etter App Store. KI er nå ~3,5 år fra ChatGPT. Vi er midt i killer-app-vinduet.

Kjennetegn på killer-app: det er ikke en ny ting, det er en gammel oppgave gjort radikalt billigere/raskere/bedre. Regneark gjorde *ikke* nytt — det gjorde regnskap 100× raskere. Søk gjorde *ikke* nytt — det gjorde biblioteksoppslag 1000× raskere. KI killer-apps blir gamle oppgaver gjort 10–100× raskere, ikke nye sci-fi-funksjoner.

For meg konkret: hva er den oppgaven i RFP-domenet som tar 40 timer i dag og kan ta 4 timer? Det er killer-app-spørsmålet. Ikke «hva kan KI gjøre?», men «hva tar 40 timer som ikke skulle tatt 40 timer?»

### 4. Standarder kommer i fase 2, lager moats i fase 3

TCP/IP, HTTP, HTML, REST. Hver av disse var omstridt før de var åpenbare. Den som bygde på riktig standard tidlig fikk uforholdsmessig avkastning (Cisco på TCP/IP, Akamai på HTTP).

KI-standardene som er i støping nå: MCP (Model Context Protocol), agent-til-agent-protokoller, eval-formater, prompt-versjonering, governance-rammeverk. Det er for tidlig å si hvilke som vinner — men det er sent å vente til de er sluttet før man velger.

For område 08: minst én eval-suite og minst ett agent-pattern må være bygget på en standard som har realistisk sjanse til å overleve 2027. Dokumenter valget. Hvis standarden dør, dokumenter migreringen.

### 5. Governance henger alltid etter — men mindre denne gangen

PC: 23 år fra IBM PC til DMCA. Internett: 25 år fra Mosaic til GDPR. KI: 2 år fra ChatGPT til EU AI Act.

Reguleringsbølgen kommer raskere fordi (a) samfunnet har lært av forrige bølge, (b) skadene synes raskere, (c) konsentrasjonen av makt er tydeligere. Det betyr at den som bygger AI-løsninger i 2026 må bygge for *kommende* regulering, ikke gjeldende.

Konkret: hvis RFP Studio brukes i tilbudsprosesser med offentlig sektor i 2027, må logging, audit-spor, modell-transparens og menneskelig overstyring være designet inn fra dag én. Etterpåklokskap er dyrt.

## Mønstre som *ikke* overføres

### 1. Tidsskalaen er komprimert

PC tok 20 år fra hobbyfase til kontorstandard. Internett tok 12. KI ser ut til å ta 4–6. Det betyr at fryktkurver, læringskurver og karrierevalg må kompresseres tilsvarende. Det jeg lærer meg på 6 måneder i dag tilsvarer 2 år av PC-æraen i strategisk verdi — men også i hvor raskt det blir foreldet.

Konsekvens for læringsplan (08): kvartalsrytme er sannsynligvis riktig granularitet. Årsrytme er for sakte. Månedsrytme er for travel.

### 2. KI er *agentisk*, ikke bare et verktøy

PC og internett var verktøy: brukeren handler, maskinen utfører. KI er en aktør: maskinen tar beslutninger, foreslår, eksekverer. Det skifter risikomodellen fundamentalt. Et regneark gjør ikke feil — det regner som du ber om. En agent kan gjøre feil i hva *den selv* tolker som oppgaven.

Det betyr at evals ikke er en QA-funksjon — det er en *kontroll*-funksjon. Tilsvarer regnskapsrevisjon, ikke programvaretest. Eval-arbeid i 08-området bør behandles deretter: alvorligere, mer formelt, med spor som tåler ettersyn.

### 3. Infrastruktur og applikasjoner bygges samtidig

PC fikk 10 år med moden hardware før applikasjonsboomen. Internett fikk 5 år med moden infrastruktur før Web 2.0. KI får null. Modeller, agent-rammeverk, evals, governance og applikasjoner bygges parallelt, av delvis overlappende team. Det betyr mer kaos, mer brudd, og mer fortjeneste til den som tåler usikkerhet.

For meg: lavere terskel for å rive opp og bygge på nytt. Det jeg bygger i Q2 2026 vil sannsynligvis være rivd ned i Q4 2026. Det er ikke feil — det er normalfasen.

### 4. Suksess er probabilistisk, ikke binær

Et program kjører eller kjører ikke. En nettside laster eller laster ikke. En agent gir godt nok svar i 87% av tilfellene. Det krever en helt annen modus: terskler, intervaller, regresjonstesting på utfall, ikke på output. Ingen tidligere bølge har trent oss på dette.

Det er derfor «evals som håndverk» står i 08-suksesskriteriene. Det er ikke teknisk pynt — det er den nye grunnferdigheten.

## Hvor er KI nå (april 2026)?

Min lesning, kalibrert mot kartet over:

- **Hobbyfasen**: ferdig (2020–22).
- **Konsumentmomentet**: ferdig (nov 2022).
- **Killer-app-vinduet**: midt i. Coding-assistenter er etablert. Andre domener (juss, RFP, design, robotikk) er fortsatt åpne.
- **Plattformkrigen**: aktiv. Vinneren ikke avgjort. Open weights tar mer plass enn forventet.
- **Distribusjonsskifte**: tidlig. Lokale modeller (Llama, Qwen, Mistral) er brukbare nå, ikke gode nok for kjernekritiske jobber ennå. 12–18 måneder unna det skiftet.
- **Governance-bølgen**: aktiv. EU AI Act i implementeringsfase. Sektorregulering kommer.
- **Embedded-fasen**: ikke startet. Kommer ~2028–2030.

Mest sannsynlige overraskelse de neste 12 månedene: en applikasjon vi ikke har sett ennå tar markedet på 6 måneder, slik regneark og søk gjorde. Det vil sannsynligvis skje i et domene der oppgaven er repetitiv, høy-volum og tekstdrevet. RFP og tilbudsarbeid er nettopp et slikt domene.

## Konsekvenser for egen plan

| Område | Implikasjon | Konkret grep neste kvartal |
|---|---|---|
| Eval-suite (RFP Studio) | Eval blir kontroll, ikke QA. Spor må tåle ettersyn. | Bygg eval-suite med audit-logg fra dag én. |
| Agent-patterns | Standarder former — MCP, agent-protokoller. | Velg én pattern bygget på MCP. Dokumenter hvorfor. |
| Lokale modeller | 12–18 mnd unna kjernekritisk bruk. | Bygg arkitektur så API-laget kan byttes ut uten å rive applikasjonen. |
| Governance | Regulering kommer raskere enn forrige bølge. | Designe inn audit, transparens, overstyring i RFP Studio nå. |
| Killer-app-jakt | 40-timersoppgaver er signalet. | List fem 40-timersoppgaver i RFP-flyten. Velg én å redusere til 4 timer. |
| Læringstempo | Kvartalsrytme er riktig granularitet. | Behold kvartalsvis baseline-oppdatering. Ikke senere, ikke oftere. |

## Anti-mønstre å unngå

- **«Denne gangen er alt annerledes.»** Det er den vanligste setningen før en boble sprekker. KI har genuine forskjeller, men kostnadskurver, plattformkriger og governance-bølger er like.
- **«Det er for tidlig å bygge.»** Var feil for PC i 1985, internett i 1996, mobil i 2008. Killer-app-vinduet lukker seg, det åpner ikke.
- **«Vi venter til standardene er satt.»** Standardene settes av de som bygger først. Ventere får tilpassningskostnaden, ikke valgfriheten.
- **«Vi velger den største leverandøren.»** Wang, DEC, AOL, Yahoo, Nokia. Alle var størst i sin fase. Velg på arkitektur, ikke på markedsandel.
- **«Vi skal ikke regulere før vi forstår.»** Forrige to bølger gjorde det. Resultatet var GDPR i panikk og antitrust 25 år for sent. Bygg som om reguleringen allerede er der.

## Når dette skal leses på nytt

- Hvert kvartal: sjekk om fasekartet fortsatt stemmer. Spesielt: er killer-app-vinduet fortsatt åpent?
- Når en ny modellgenerasjon slipper: re-evaluer «lokale modeller»-tidslinjen.
- Når EU AI Act-håndhevingen begynner (forventet 2026–27): re-evaluer governance-radet.
- Når RFP Studio når 100 brukere: revurder killer-app-hypotesen — er 40-timersoppgaven faktisk redusert?

# Kompetanseplattform — Spec

## Formål

En personlig, strukturert utviklingsplattform for soft skills og fremtidskritiske ferdigheter. Målet er ikke å lese mer — det er å operasjonalisere lesing til handling, koble hvert område til konkrete jobbsituasjoner (PFT, RFP Studio, foredrag, workshops), og spore reell progresjon over tid.

Horisont: 2026–2030. Koblet mot eksisterende kompetanseplan (ADKAR-rammeverk, lønnsmål 900k–1M+, ledermål innen 2029–2030).

## Designprinsipper

- **Praksis over pensum.** Hvert område må koble til en pågående eller nylig jobbsituasjon. Hvis ikke, hører det ikke hjemme her.
- **Baseline først, mål fremover.** Selvevaluering i starten. Kvartalsvis reevaluering. Progresjon er data, ikke følelse.
- **Refleksjon commites.** Alle læringslogger i git — så mønstre over tid blir synlige.
- **Få nok, ikke for mye.** Ti kjerneområder. Ikke tjue.
- **Append-only refleksjon.** Dagbokinnlegg redigeres ikke. Feil tenkning fra i fjor er data, ikke flauhet.
- **Privat først.** Repoet er privat. Enkeltinnsikter kan promoteres til LinkedIn-artikler senere.

## Mappestruktur

```
kompetanseplattform/
├── README.md
├── SPEC.md
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── laeringsmaal.md
│       ├── refleksjon.md
│       └── bok-oppsummering.md
├── 00-oversikt/
│   ├── baseline-2026.md
│   ├── maal-2026-2030.md
│   ├── progresjon-kvartal.md
│   └── dashboard.md
├── 01-eq-emosjonell-intelligens/
├── 02-psykologi-og-atferd/
├── 03-endringsledelse-i-praksis/
├── 04-innflytelse-og-vanskelige-samtaler/
├── 05-skriftlig-klarhet-for-beslutningstakere/
├── 06-multiplikator-ledelse-og-coaching/
├── 07-portefolje-og-strategisk-tenkning/
├── 08-fremtidskritiske-ferdigheter/
├── 09-ux-og-brukerdesign/
├── 10-storytelling-og-foredragsholding/
├── lederdagbok/
│   ├── 2026-Q2/
│   └── README.md
├── lesestoff/
│   ├── bibliotek.md
│   ├── kø.md
│   └── notater/
└── scripts/
    ├── ukes-prompt.md
    └── kvartal-gjennomgang.md
```

## Per-område mal

Hvert kjerneområde (01- til 08-) har identisk intern struktur:

```
0X-omradenavn/
├── README.md          Hva er dette? Hvorfor matters for deg spesifikt?
├── baseline.md        Selvevaluering 1–5 per delferdighet, med dato
├── pensum.md          Bøker/kurs/artikler, prioritert
├── praksis.md         Konkrete øvelser koblet til jobbsituasjoner
├── refleksjon.md      Append-only logg
├── maal.md            Hva skal være annerledes om 12 mnd?
└── ressurser/         Notater fra bøker, utklipp, modeller
```

## Kjerneområdene

### 01 — EQ / Emosjonell intelligens

**Hvorfor:** Høy self-awareness, umoden self-regulation. Systemer for å navigere svingninger i innovasjonsdriv og motivasjon.

Delferdigheter: Self-awareness · Self-regulation · Intrinsisk motivasjon · Empati · Sosial ferdighet.

Pensum (prioritert): Emotional Intelligence 2.0 (Bradberry & Greaves) · Working with Emotional Intelligence (Goleman) · Permission to Feel (Brackett) · The Body Keeps the Score (van der Kolk).

Praksis: daglig 2-min emotional labeling · før/etter-refleksjon på workshops · månedlig 360-light (Thomas, Elin, +1).

### 02 — Psykologi og atferd

**Hvorfor:** Fra "kjenner biasene" til "ser biasene i sanntid hos meg og andre".

Delferdigheter: gjenkjenne egne bias · etisk nudging · lese gruppedynamikk · motivasjonsarkitektur (SDT, Pink).

Pensum: Thinking, Fast and Slow (Kahneman) · Nudge (Thaler & Sunstein) · Drive (Pink) · Predictably Irrational (Ariely) · The Elephant in the Brain · Influence (Cialdini).

Praksis: pre-workshop bias-prediksjon · post-RFP Studio bias-diagnose · månedlig "jeg tok feil"-innlegg.

### 03 — Endringsledelse i praksis

**Hvorfor:** Fra taksonomi til intervensjon. Når en navngitt person står fast i motstand, hvilket grep tar du?

Delferdigheter: diagnostisere motstand (ADKAR) · løpende stakeholder-map · tilpasse argumentasjon til arketype · designe sponsorships.

Pensum: Switch · Leading Change · Immunity to Change · The Change Monster · Prosci ADKAR Practitioner.

Praksis: `stakeholder-map.md` for pågående PFT-endring · 4-ukers ADKAR-intervensjon på én person · reversert Kotter-diagnose.

### 04 — Innflytelse og vanskelige samtaler

**Hvorfor:** Diplomatisk default. Senior Advisor-rollen krever å levere ubehag uten å miste relasjonen.

Delferdigheter: si nei uten relasjonsskade · korrigerende feedback ansikt-til-ansikt · lede unngått samtale · forhandle scope/mandat · motstå påvirkningsteknikker.

Pensum: Crucial Conversations · Never Split the Difference · Nonviolent Communication · Thanks for the Feedback · Negotiating the Impossible · Influence.

Praksis: utsatt samtale tatt innen 7 dager · månedlig "kalibrert no" · rollespill med Claude før reelle samtaler.

### 05 — Skriftlig klarhet for beslutningstakere

**Hvorfor:** Valutaen på 900k+ er én side direktøren signerer uten spørsmål.

Delferdigheter: BLUF · Amazon 6-pager · PR/FAQ · Situation-Complication-Resolution · beslutningsnotat på én A4.

Pensum: On Writing Well · Made to Stick · The Pyramid Principle (Minto) · Writing Without Bullshit · Working Backwards (Bryar).

Praksis: ukentlig A4-beslutningsnotat (ikke send) · barber langt notat til 250 ord · månedlig review fra Thomas.

### 06 — Multiplikator-ledelse og coaching

**Hvorfor:** Fra svar-modus til å utvikle andre. Pre-rekvisitt til lederrolle 2029–2030.

Delferdigheter: spørsmål du ikke vet svaret på · Coaching Habit-modellen · delegering som utvikling · unngå Diminisher-mønstre.

Pensum: Multipliers · The Coaching Habit · Humble Inquiry · The Making of a Manager · Staff Engineer.

Praksis: ett ukjent-svar-spørsmål per 1:1 · månedlig delegerings-øvelse · kvartalsvis duo-leveranse i stedet for solo.

### 07 — Portefølje og strategisk tenkning

**Hvorfor:** Fra å levere prosjekter til å prioritere på tvers og si nei. Uten dette forblir du beste senior-advisor, ikke leder av området.

Delferdigheter: Wardley Mapping · OKRs på riktig nivå · good vs bad strategy · si nei til gode idéer.

Pensum: Good Strategy/Bad Strategy · Wardley Maps · Measure What Matters · The Art of Action · Essentialism.

Praksis: Wardley Map for PFT Eiendoms AI-portefølje · 3 personlige OKRs for H2 2026 · månedlig "ikke-liste".

### 08 — Fremtidskritiske ferdigheter

**Hvorfor:** Der teknisk bredde allerede er sterk, men skillet mellom "henger med" og "definerer kanten" er tynt.

Delferdigheter: evals som håndverk · agent-arkitektur utover Plan-and-Execute · lokale/on-prem modeller · AI governance som drift · spatial/multimodal AI for PropTech.

Kilder: Hamel Husains skriverier om evals · Anthropic engineering blogg · Chip Huyen, AI Engineering · Simon Willisons blogg · Latent Space · IAPP AIGP BoK v2.1.

Praksis: eval-suite for RFP Studio · månedlig agent-pattern-eksperiment · månedlig teknisk LinkedIn-artikkel.

### 09 — UX og brukerdesign

**Hvorfor:** Bygger interne AI-produkter og fasiliterer workshops, men argumenterer for hva jeg tror brukere trenger — ikke hva jeg har observert. AI-UX er umodent felt; tidlig posisjonering gir fortrinn.

Delferdigheter: bruker-interview som metode · jobs-to-be-done · informasjonsarkitektur og flyt · prototyping (wireframe-nivå) · usability testing · microcopy · accessibility-grunnlag · AI-UX (confidence, kontroll, feilmoduser).

Pensum: Don't Make Me Think (Krug) · The Design of Everyday Things (Norman) · Just Enough Research (Hall) · Articulating Design Decisions (Greever) · 100 Things Every Designer Needs to Know About People (Weinschenk) · levende kilder for AI-UX (NN/g, Apple HIG, Material, Anthropic/OpenAI).

Praksis: månedlig bruker-interview · månedlig usability-test · kvartalsvis service blueprint · kvartalsvis AI-UX-pattern-eksperiment.

Overlapp håndteres bevisst: microcopy → 05, kognitive bias → 02, produksjonsnære AI-patterns → 08.

### 10 — Storytelling og foredragsholding

**Hvorfor:** Holder allerede foredrag og fasiliterer workshops. Gapet mellom "gode foredrag" og "hendelser folk husker og omtaler" er det som skiller intern synlighet fra ekstern etterspørsel. Multiplikator for 04, 05 og 08.

Delferdigheter: narrativ struktur · åpninger og avslutninger · egen historiebank med moral · tempo, pauser, stemmebruk · lese rommet · data som historie · Q&A under press · workshop-fasilitering.

Pensum: Resonate (Duarte) · Storyworthy (Dicks) · Talk Like TED (Gallo) · Confessions of a Public Speaker (Berkun) · The Art of Gathering (Parker). Levende: TED-dekonstruksjoner, Moth Radio Hour.

Praksis: kontinuerlig vedlikeholdt historiebank (mål ≥20 anekdoter) · per foredrag: 30-sek pitch, åpning/avslutning øvd høyt, post-mortem · kvartalsvis: video-opptak sett tilbake · kvartalsvis: TED-dekonstruksjon.

Overlapp: BLUF-struktur → 05, publikum-bias → 02, fasiliteringsspørsmål som utvikler andre → 06.

## Baseline-mal

For hvert område, skår deg selv 1–5 per delferdighet. Oppdater kvartalsvis. Commit-melding: `baseline: Q2 2026`.

## Refleksjon — format

`refleksjon.md` i hvert område er append-only:

```
## YYYY-MM-DD

Situasjon: [kort]
Hva jeg gjorde: [kort]
Hva som skjedde: [kort]
Hva dette lærer meg: [1–3 setninger]
Hva jeg prøver annerledes neste gang: [konkret]
```

Redigeres aldri. Feil analyse er data.

## Lederdagbok

`lederdagbok/YYYY-QN/YYYY-MM-DD.md`. Ukentlig til månedlig:

1. Én situasjon der jeg tok en lederrolle (formell/uformell).
2. Én situasjon der jeg burde tatt en lederrolle, men lot være.
3. Én observasjon av en leder rundt meg (Thomas, eksterne).

Råvare til selvevaluering og senere LinkedIn-innhold.

## Issue templates

- `laeringsmaal.md`: "Jeg vil kunne X innen dato Y. Måling: Z. Område: 0N."
- `refleksjon.md`: kvartalsvis refleksjon på tvers.
- `bok-oppsummering.md`: hovedbudskap, 3 nøkkelinnsikter, 1 ting jeg skal prøve, jobb-kobling.

Labels: `omrade-01` – `omrade-10`, `kvartal-Q2-2026`, `bok`, `praksis`, `refleksjon`. Lukket issue = fullført mål.

## Dashboard

`00-oversikt/dashboard.md` — manuell Markdown-tabell, oppdateres kvartalsvis. Kolonner: Område · Baseline Q2 · Q3 · Q4 · Q1 2027 · Hovedfokus kommende kvartal.

## Kvartalsrytme

- **Ukentlig**: én refleksjonslogg i aktivt område.
- **Månedlig**: én boknotat · ett A4-beslutningsnotat (øvelse) · én vanskelig samtale · én "ikke-liste".
- **Kvartalsvis**: oppdater baseline for alle 10 · oppdater dashboard · 500-ords refleksjon i `progresjon-kvartal.md` · velg primær/sekundær-område · vurder LinkedIn-innlegg.
- **Årlig**: full gjennomgang + kobling mot lønnsforhandling / karrieresamtale med Thomas.

## Claude Code-workflows

- **Scaffolding**: "Les SPEC.md og opprett strukturen."
- **Refleksjon**: "Gi refleksjonslogg-mal for område X basert på situasjon Y."
- **Bokoppsummering**: "Jeg har lest [bok]. Generer notat etter bok-oppsummering-template."
- **Stakeholder-map**: "Oppdater stakeholder-map.md basert på disse notatene."
- **Kvartalsgjennomgang**: "Les alle `refleksjon.md` og foreslå mønstre, tilbakevendende temaer, blindflekker."

## Suksesskriterier (12 mnd)

- Baseline-skår opp minst 1 poeng i minst 4 av 10 områder.
- ≥40 refleksjonslogger totalt (≈ukentlig).
- ≥12 bok-oppsummeringer.
- ≥4 LinkedIn-artikler promotert fra repoet.
- ≥1 "ville ikke tatt før"-samtale tatt og logget.
- Thomas bekrefter endring i minst ett spesifikt område.

Hvis ingen av disse er sanne etter 12 mnd: plattformen er pensum, ikke praksis. Kutt strukturen, ikke utvid.

## Anti-mønstre

- **Pensum-inflasjon.** 5 nye bøker er ikke progresjon. 1 anvendt er.
- **Meta-arbeid over arbeid.** Å redesigne plattformen er ikke utvikling. Refleksjonslogger er.
- **Bare tekniske områder.** Hvis 80% av commits er i 08, er plattformen dysfunksjonell — ikke komfortabel.
- **Perfeksjon i baseline.** Skår raskt og ærlig. 3 er ikke en fornærmelse, det er data.

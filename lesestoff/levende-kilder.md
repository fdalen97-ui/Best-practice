# Levende kilder

Åpne ressurser som oppdateres løpende, ikke bøker. Brukes når et område trenger **applisert, dagsaktuell** kunnskap (UX-mønstre, tilgjengelighetskrav, designsystem-detaljer) der boklister blir for trege.

Skilles bevisst fra `bibliotek.md` (fullførte bøker) og `kø.md` (aktive bøker).

## Policy

- Tas inn kun når en **konkret jobbsituasjon** krever det. Ikke samles "for å være oppdatert".
- Hver kilde skal ha **én eier-område** og **én forventet bruksmåte**. Ellers er den støy.
- Når kilden faktisk brukes (i sak, refleksjon, beslutning) → notér i `<område>/ressurser/`.
- Levende kilder skal *avkorte* arbeid, ikke utvide det.

## Norsk offentlig sektor

Konkrete repoer plukket fordi de er aktivt vedlikeholdt og direkte anvendbare. Ikke en oversikt — et utvalg.

| Kilde | Område | Bruksmåte |
|---|---|---|
| [navikt/aksel](https://github.com/navikt/aksel) — Navs designsystem og Aksel-portalen | 09 UX | Slå opp komponent-mønstre og UU-tekst når RFP Studio-skisser tas til review. Sammenlign, ikke kopier. |
| [digdir/designsystemet](https://github.com/digdir/designsystemet) — Digdirs designsystem | 09 UX | Referanse på norsk språkbruk og skjemaflyt i offentlig tjenestekontekst. |
| [navikt/universell-utforming](https://github.com/navikt/universell-utforming) — NAV-veileder for UU i utviklingsteam | 09 UX | Praktisk sjekkliste når trunk-test avdekker svakheter. Korter ned WCAG til tiltak. Eldre, men prinsippene står. |
| [entur/design-system](https://github.com/entur/design-system) — Entur Linje | 09 UX | Sekundærreferanse — transportdomenet er smalt, men konsistens-prinsippene er overførbare. |

## Eksempel på god bruk

**Situasjon**: Du vurderer om en knapp-plassering i RFP Studio er forvirrende.

- **Dårlig bruk**: Lese gjennom hele Aksel-portalen "for å være forberedt".
- **God bruk**: Søk konkret etter `primary action` i Aksel, sammenlign med din skisse, skriv én notat i `09-ux-og-brukerdesign/ressurser/aksel-knapp-pattern-YYYY-MM.md` med beslutning og begrunnelse. Lukk fanen.

## Anti-mønstre

- Listen blir til en lenke-samling som aldri brukes.
- Kilder lagt inn fordi de "burde" være med, ikke fordi en oppgave krever dem.
- Boknotat-mal brukt på levende kilder — feil format. Levende kilder skal logges *per bruk*, ikke *per kilde*.

# Full-stack — hva det faktisk betyr

Kilde: DeCodeDev-infografikk på Instagram/TikTok.

## Hovedpoeng

"Full-stack" blir ofte misforstått som "frontend + backend". I praksis er det en stabel med 10–12 lag, der hvert lag har eget fag og egne feilmoduser. Du trenger ikke være ekspert på alle, men du må vite hva hvert lag *gjør*, slik at du vet hvem du skal spørre og hvor feil oppstår.

## De 12 lagene — forklart

| # | Lag | Hva det er | Typisk teknologi | Hva ryker hvis det feiler |
|---|---|---|---|---|
| 1 | **Frontend** | Det brukeren ser og klikker på i nettleseren/appen. | React, Vue, Svelte, HTML/CSS | Brukeren ser "white screen", knapper virker ikke |
| 2 | **Backend / APIs** | Serverlogikk som tar imot forespørsler og gir svar. "Hjernen." | Node.js, Python, Go, Java | Frontend får 500-feil, ingen data kommer ut |
| 3 | **Database** | Der data lagres permanent. | Postgres, MySQL, MongoDB | Ingenting huskes mellom økter |
| 4 | **Servers** | De fysiske/virtuelle maskinene som kjører koden. | EC2-instans, bare-metal, VM | Alt går ned |
| 5 | **Networking** | Hvordan trafikk finner frem. DNS, lastbalansering, brannmur. | Nginx, Cloudflare, HAProxy | Noen brukere får ikke kontakt, latency øker |
| 6 | **Cloud Infrastructure** | Skyplattformen maskinene kjører på. | AWS, Azure, GCP | Regninger eksploderer, regions-utfall |
| 7 | **CI/CD Pipelines** | Automatisk bygging, testing og utrulling av kode. | GitHub Actions, GitLab CI, Jenkins | Ingen ny kode kommer ut i produksjon |
| 8 | **Security** | Autentisering, autorisasjon, kryptering, patching. | OAuth, TLS, secrets-håndtering | Hendelse. Stort bilde, mye å rydde |
| 9 | **Containers** | Pakke koden + avhengigheter som én kjørbar enhet. | Docker, Kubernetes | "Works on my machine"-problemer, utrulling bryter |
| 10 | **CDN** | Kopier av statiske filer nærmere brukeren geografisk. | Cloudflare, Fastly, CloudFront | Tregt globalt, spesielt bilder/video |
| 11 | **Monitoring & Logging** | Ser hva som faktisk skjer i prod, i sanntid. | Grafana, Datadog, Sentry, ELK | Du vet ikke at noe er galt før brukeren klager |
| 12 | **Backups & Recovery** | Kopier av data + plan for å komme tilbake etter katastrofe. | Point-in-time recovery, snapshots | Data tapt for alltid |

> **Merknad**: Infografikken viser "Containers" to ganger. Trolig en grafisk feil — lag 11 i originalen skulle sannsynligvis vært **Load Balancer** eller **Queues/Messaging** (Kafka, RabbitMQ, SQS). Verdt å sjekke om du ser bildet på nytt.

## Hvordan lagene henger sammen

```
Brukeren
   ↓
Frontend (nettleser)
   ↓                    ← CDN cacher statiske filer
Networking (DNS, LB)
   ↓
Backend / API           ← kjører i Container
   ↓
Database
```

*Under alt dette*: Cloud infrastructure (maskinene), Security (gjennom hele stacken), CI/CD (hvordan det havner der), Monitoring (hvordan du vet det virker), Backups (hva som skjer når det ikke virker).

## Hvorfor dette er nyttig for meg

Jeg skriver ikke kode full-stack selv, men:
- **Når jeg snakker med utviklere om RFP Studio / PFT**: jeg kan stille riktige spørsmål ("Hvem eier monitoring-laget?" "Er CI/CD koblet til evals?").
- **Når jeg vurderer leverandører / konsulenthus**: jeg kan høre forskjell på en "fullstack-utvikler" som bare kan lag 1–2 og en som også vet 5–12.
- **Når noe går galt i produksjon**: jeg kan lokalisere hvor feilen *sannsynligvis* sitter før jeg eskalerer.
- **For eval-arbeidet (område 08)**: evals lever i CI/CD-laget. Monitoring og logging gir deg signal når evals faller. Uten disse lagene er evals teater.

## 1 ting jeg skal prøve

*(Fyll inn: f.eks. "I neste teknisk review: pek på hvilket lag hver risiko hører hjemme i, innen 30.05.")*

## Forståelsesvurdering

Dette notatet er en **referanse jeg lager til meg selv**, ikke et notat fra en gjennomgang. Forståelsesnivå pr. nå:

- **Lag 1–4 (Frontend, Backend, DB, Servers)**: konseptuelt solid. Kan forklare til ikke-tekniske.
- **Lag 5–7 (Networking, Cloud, CI/CD)**: forstår rollen, men detaljene (DNS-flyt, skyregion-valg, pipeline-design) krever oppslag.
- **Lag 8–10 (Security, Containers, CDN)**: konseptuelt greit, praktisk tynt. Har aldri skrevet en Dockerfile selv.
- **Lag 11–12 (Monitoring, Backups)**: vet hvorfor de finnes, vet lite om hvordan de settes opp bra.

**Neste steg hvis jeg vil bygge dypere**: velg ett lag jeg er svakest på per kvartal (f.eks. CI/CD Q2) og les én god artikkel + sett opp én mini-demo selv.

## Område

- [x] omrade-08 Fremtidskritiske ferdigheter *(foundation, ikke frontier)*

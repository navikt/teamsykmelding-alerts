[![Build status](https://github.com/navikt/sykmelding-alerts/workflows/Deploy%20to%20dev%20and%20prod/badge.svg)](https://github.com/navikt/sykmelding-alerts/workflows/Deploy%20to%20dev%20and%20prod/badge.svg)

# sykmelding-alerts

Lager alerts for team sykmelding sine apper

For mer informasjon om hvordan alarmene fungerer se:
`https://doc.nais.io/observability/alerts/`

## Utvikling
### GCP
En kan bruke `https://prometheus.dev-gcp.nav.cloud.nais.io/` som hjelp til å teste queries.
### FSS
En kan bruke `https://prometheus.dev-fss.nav.cloud.nais.io/` som hjelp til å teste queries.

### Deploy prod
Alle kode som er i master går til prod-gcp og prod-fss
### GCP
Dette kan evt gjøres manuelt med følgende kommando:
`kubectl apply --context prod-gcp --namespace default -f sykmeldingalerts.yaml`
### FSS
Dette kan evt gjøres manuelt med følgende kommando:
`kubectl apply --context prod-fss --namespace default -f sykmeldingalerts.yaml`

## Henvendelser
Dette prosjeket er vedlikeholdt av [navikt/teamsykmelding](CODEOWNERS)

Spørsmål knyttet til koden eller prosjektet kan stilles som
[issues](https://github.com/navikt/sykmelding-alerts/issues) her på GitHub

### For NAV-ansatte
Interne henvendelser kan sendes via Slack i kanalen [#team-sykmelding](https://nav-it.slack.com/archives/CMA3XV997)
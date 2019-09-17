# sykmelding-alerts

Lager alerts for team sykmelding sine apper

For mer informasjon om hvordan alarmene fungere se:
`https://github.com/nais/doc/tree/master/content/alerts`

## Utvikling:
En kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries.

### Deploy prod:
All kode som blir er i master går til prod, når github actions er oppe og går
Kan i mellomtiden gjøres manuelt med følgende kommando:
`kubectl apply --context prod-fss --namespace default -f sykmeldingalerts.yaml`

### For NAV ansatte
Vi er tilgjenngelig på slack kanalen #team-sykmelding
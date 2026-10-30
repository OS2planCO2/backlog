# Issue-skabeloner til OS2planCO2

Disse skabeloner bruges i [OS2planCO2/backlog](https://github.com/OS2planCO2/backlog) til fejl, udviklingsønsker og brugerhistorier. Backlog og projektstyring er adskilt fra [kildekoden til QGIS-pluginet](https://github.com/OS2planCO2/planCO2).

OS2planCO2 beregner CO₂-aftryk for bygninger, veje og åbne arealer som støtte til planlægning. Se [brugervejledningen](https://github.com/OS2planCO2/planCO2/blob/main/docs/PlanCO2_Guide.pdf).

## Placering

Kopiér de fem filer til denne mappe i **backlog-repositoryet**:

```text
.github/
└── ISSUE_TEMPLATE/
    ├── README.md
    ├── bug_report.yml
    ├── feature_request.yml
    ├── user_story.yml
    └── config.yml
```

ZIP-pakken indeholder allerede denne mappestruktur. Ved udpakning skal skjulte mapper medtages. Denne README er vejledning til skabelonerne og skal ligge i `.github/ISSUE_TEMPLATE/`; den erstatter ikke repositoryets README i roden.

De fire YAML-filer skal ligge på repositoryets standardbranch, før GitHub viser formularerne under **Issues → New issue**. Der skal være aktiveret Issues i repositoryet. Der er ikke behov for hjælpefiler eller tomme mapper.

## Vælg skabelon

| Fil | Anvendelse |
| --- | --- |
| `bug_report.yml` | En fejl eller et uventet resultat. Angiv QGIS-version, plugin-version, operativsystem, trin til genskabelse samt faktisk og forventet adfærd. Tilføj relevante data og beregningsindstillinger. |
| `feature_request.yml` | Et nyt behov eller en forbedring. Beskriv nuværende arbejdsgang, ønsket ændring, målgruppe og værdi. |
| `user_story.yml` | Et afgrænset brugerbehov med testbare acceptkriterier i formen Givet–Når–Så. |
| `config.yml` | Styrer skabelonvælgeren og giver links til sikkerhedspolitik, brugervejledning og kildekode. |

Søg i både åbne og lukkede sager før oprettelse. Brug kommentarer til opfølgning og testresultater. Fejlrapporter og brugerhistorier indeholder en forudfyldt testvejledning med versionsoplysninger, testdata og forventede kontra faktiske resultater. Feltet og den oprettede sagsbeskrivelse kan redigeres; GitHub låser ikke teksten.

## Opsætning og tilpasninger

- `blank_issues_enabled: false` leder almindelige bidragydere til formularerne. Brugere med skriverettigheder eller højere kan fortsat oprette tomme sager.
- Formularerne bruger titelpræfikser. Automatisk tildeling af labels, sagstyper, personer og Projects er udeladt, så filerne kan bruges uden yderligere opsætning. Det kan tilføjes senere med eksisterende labels og sagstyper samt et konkret projekt i formatet `OS2planCO2/<projektnummer>`.
- Dublerede `projects`-nøgler, OS2valghalla-henvisninger og den udokumenterede `body_only`-nøgle er fjernet. Felter til side-URL og browser er erstattet af oplysninger om QGIS, plugin og data. Der er ikke fastsat en ny behandlingsfrekvens eller særlige statusnavne.
- Navn og e-mail er ikke obligatoriske felter. Opfølgning sker via GitHub-kontoen. Kommune eller organisation er valgfri i udviklingsønsker. Del kun data, logfiler og projektfiler, som må offentliggøres.

Retningslinjer: [Bidrag](../../CONTRIBUTING.md), [adfærdskodeks](../../CODE_OF_CONDUCT.md), [governance](../../GOVERNANCE.md) og [sikkerhed](../../SECURITY.md). Licenser findes i [LICENSE](../../LICENSE) og [LICENSE-DOCS](../../LICENSE-DOCS).

Sikkerhedssårbarheder indberettes efter [SECURITY.md](../../SECURITY.md): **os2planco2@os2.eu** med kopi til **security@os2.eu**.

## Kontrol før brug

Filerne er kontrolleret lokalt for YAML-syntaks, dublerede nøgler, formularstruktur, entydige felt-id'er og henvisninger. Kontrollen følger GitHubs dokumentation for [issue-formularer](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms), [formularfelter](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-githubs-form-schema) og [skabelonvælgeren](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository).

Efter tilføjelse til standardbranchen bør de tre formularer åbnes via **New issue** for at kontrollere visning og obligatoriske felter. GitHubs egen visning er ikke afprøvet som del af denne levering; der er ikke foretaget ændringer på GitHub.

### English summary

These Danish issue forms support the OS2planCO2 backlog, separately from the QGIS plugin source code. Place all five files in `.github/ISSUE_TEMPLATE/` in the backlog repository. Report security vulnerabilities according to the repository's security policy.

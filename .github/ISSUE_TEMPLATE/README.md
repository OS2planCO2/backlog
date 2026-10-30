# Issue-skabeloner

Denne mappe indeholder de issue-skabeloner, der kan bruges til at oprette issues i et repository.

Skabelonerne gør det nemmere at oprette issues med en ensartet struktur og sikrer, at de nødvendige oplysninger er med, når man indberetter fejl, foreslår nye funktioner eller beskriver brugerhistorier.

## Mappestruktur

For at skabelonerne fungerer, skal mapper og filnavne placeres og navngives **præcist som beskrevet nedenfor** i det repository, hvor de skal bruges:

```text
.github/
└── ISSUE_TEMPLATE/
    ├── config.yml
    ├── bug_report.yml
    ├── feature_request.yml
    └── user_story.yml
```

Der kan tilføjes flere skabeloner efter behov, fx:

```text
    ├── epic.yml
    └── task.yml
```

## Sådan opsættes skabelonerne

Mappen `ISSUE_TEMPLATE` skal ligge i en mappe med navnet `.github` i **roden af det repository, hvor skabelonerne skal bruges**.

### 1. Opret mappen `.github`

Opret en mappe med navnet:

```text
.github
```

Mappen skal ligge i roden af repositoryet.

Når du opretter mappen direkte i GitHub, skal du samtidig oprette en fil, da en mappe ikke kan være tom. Du kan fx oprette:

```text
.github/issues.md
```

Vælg **Add file → Create new file**, og indtast `.github/issues.md` i filnavnefeltet. Filen kan efterfølgende bruges eller slettes efter behov.

### 2. Opret mappen `ISSUE_TEMPLATE`

Opret en undermappe i `.github` med navnet:

```text
ISSUE_TEMPLATE
```

Navnet skal skrives præcist som vist, inklusive understregningen og de store bogstaver.

Mappen skal indeholde mindst én fil. Du kan passende starte med `config.yml`.

### 3. Tilføj issue-skabelonerne

Følgende skabeloner er klar til brug og kan kopieres fra denne mappe til `ISSUE_TEMPLATE`:

- `bug_report.yml` – til indberetning af fejl
- `feature_request.yml` – til forslag om nye funktioner
- `user_story.yml` – til beskrivelse af funktionalitet ud fra brugerens perspektiv
- `config.yml` – konfiguration af visningen af issue-skabelonerne

Filerne er klargjorte skabeloner, der kan kopieres direkte til et repository.

Der kan også oprettes yderligere skabeloner efter behov:

- `epic.yml` – til større opgaver, der består af flere issues
- `task.yml` – til mindre eller mere specifikke opgaver

`epic.yml` og `task.yml` er **ikke inkluderet som færdige skabeloner**, men kan oprettes og tilføjes, hvis projektet har behov for dem.

## Brug af skabelonerne

Når mappestrukturen `.github/ISSUE_TEMPLATE` er oprettet, og skabelonfilerne er tilføjet, vil skabelonerne være tilgængelige, når man vælger **New issue** i GitHub-repositoryet.

Brugeren kan herefter vælge den relevante skabelon, når et nyt issue oprettes.

## ⚠️ Vigtigt

Placering og navngivning er afgørende. GitHub genkender kun issue-skabelonerne, når de ligger på den forventede placering:

`.github/ISSUE_TEMPLATE/`

Omdøb ikke `.github` eller `ISSUE_TEMPLATE`, da GitHub så ikke kan genkende skabelonerne.

⚠️ **GDPR:** `bug_report.yml` og `feature_request.yml` beder indmelderen om navn og e-mailadresse. I offentlige repositories bør dette vurderes af hensyn til GDPR. Fjern felterne fra skabelonerne, hvis I ikke ønsker at indsamle disse oplysninger.

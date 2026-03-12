# /nyt-komma

En Claude Code skill der giver Claude styr på dansk kommasætning efter **Nyt Komma**-reglerne.

## Hvad er det?

Danske kommaregler er svære -- selv for AI. Denne skill giver Claude et komplet regelsæt, en beslutningslogik og hundredvis af eksempler, så den kan:

- **Skrive dansk tekst** med korrekt kommatering fra start
- **Rette kommaer** i eksisterende tekst og forklare hver ændring

## Installation

Klon repoet og kopier skill-mappen til din Claude Code skills-mappe:

```bash
git clone https://github.com/mikkelkrogsholm/nyt-komma.git /tmp/nyt-komma-repo
mkdir -p ~/.claude/skills/nyt-komma
cp -r /tmp/nyt-komma-repo/nyt-komma/. ~/.claude/skills/nyt-komma/
```

Du kan også installere den per projekt i stedet for globalt:

```bash
mkdir -p .claude/skills/nyt-komma
cp -r /tmp/nyt-komma-repo/nyt-komma/. .claude/skills/nyt-komma/
```

## Brug

Når skillen er installeret, aktiveres den automatisk når du beder Claude om hjælp med dansk kommatering:

```
> Ret kommaerne i denne tekst: "Min søster der bor i København fortalte mig
  at hun havde set en film som var rigtig god."
```

```
> Skriv en mail til min chef om at jeg er syg i morgen. Korrekt kommatering tak.
```

Du kan også aktivere den eksplicit:

```
> /nyt-komma Ret denne tekst: ...
```

## Hvad dækker skillen?

Skillen er baseret på **Nyt Komma**, som er den anbefalede standard i Danmark i dag. Den dækker 18 regelkategorier:

| # | Regel | Type |
|---|---|---|
| 1 | Opremsningskomma | Obligatorisk |
| 2 | Helsætningskomma | Obligatorisk |
| 3 | Ledsætningskomma (slutkomma) | Obligatorisk |
| 4 | Relativsætninger (parentetiske) | Obligatorisk |
| 5 | Appositionskomma | Obligatorisk |
| 6 | Adjektivkomma | Betinget |
| 7 | Feltseparationskomma | Betinget |
| 8 | Anført tale | Obligatorisk |
| 9 | Sætningskløvning | Valgfrit |
| 10 | Sætningsknuder | Valgfrit |
| 11 | Infinitivkonstruktioner | Forbudt |
| 12 | Ufuldstændige sætninger | Betinget |
| 13 | Selvstændige sætningsdele | Betinget |
| 14 | Særfeltskomma | Betinget |
| 15 | Modsætningskomma | Valgfrit |
| 16 | Sammenligningskomma | Valgfrit |
| 17 | Sideordningskomma | Betinget |
| 18 | Forbudte kommaer | Forbudt |

## Nyt Komma vs. Grammatisk Komma

Den vigtigste forskel: **startkomma** (komma *foran* en ledsætning) er valgfrit i Nyt Komma, mens **slutkomma** (komma *efter* en ledsætning) altid er obligatorisk. Denne skill udelader som udgangspunkt startkomma foran integrerede ledsætninger.

## Filstruktur

```
nyt-komma/
├── SKILL.md                        # Hovedfil: proces, beslutningslogik, faldgruber
└── references/
    ├── nyt_komma_regler.md         # Komplet regelsæt (18 regler)
    └── eksempler.md                # Eksempler med korrekt/forkert for hver regel
```

## Bidrag

PR's er velkomne. Hvis du finder en kommafejl i skillen selv, er det jo lidt pinligt -- men vi tager imod rettelser med kyshånd.

## Licens

MIT

---
name: grammatisk-komma
description: Dansk kommasætning efter Grammatisk Komma (traditionelt komma med startkomma). Brug denne skill når brugeren beder om hjælp med dansk kommatering med startkomma, vil have rettet kommaer i en tekst med grammatisk/traditionelt komma, eller beder dig skrive dansk tekst med startkomma. Triggerer når brugeren nævner "grammatisk komma", "traditionelt komma", "startkomma", "komma foran ledsætninger", eller specifikt beder om den traditionelle kommatering som bruges i trykte medier, aviser og journalistik. Brug den proaktivt når brugeren eksplicit beder om startkomma.
---

# Grammatisk Komma – Dansk kommasætning med startkomma

Du er en ekspert i dansk kommasætning efter Grammatisk Komma-reglerne (også kaldet traditionelt komma). Den afgørende forskel fra Nyt Komma er, at du **altid sætter startkomma foran ledsætninger**.

## Før du starter

Læs ALTID filen `references/grammatisk_komma_regler.md` før du begynder at arbejde med kommaer. Den indeholder det komplette regelsæt. Spring den ikke over – selv erfarne sprogbrugere laver kommafejl, og reglerne har mange nuancer som er nemme at overse.

Læs også `references/eksempler.md` for konkrete eksempler på hver regel.

## Grundlæggende begreber

For at anvende kommareglerne korrekt skal du kunne identificere disse sætningstyper:

**Helsætning:** En selvstændig sætning med sit eget grundled (subjekt) og udsagnsled (finit verbum i bøjet form). En helsætning kan stå alene og give mening. Eksempel: "Solen skinner" og "børnene leger" er begge helsætninger.

**Ledsætning:** En underordnet sætning der fungerer som led i en anden sætning. Ledsætninger indledes typisk af et underordningsbindeord (at, fordi, hvis, selvom, da, når, mens osv.) eller et hv-ord (hvem, hvad, hvilken, hvor, hvordan osv.). Ledsætninger kan ikke stå alene. Eksempel: I "Jeg tror, at han kommer" er "at han kommer" en ledsætning.

**Ikke-prøven:** Du kan skelne helsætninger fra ledsætninger ved at indsætte *ikke* i sætningen. I en helsætning står *ikke* **efter** udsagnsleddet. I en ledsætning står *ikke* **før** udsagnsleddet. Eksempel: "Pigen græder *ikke*" (helsætning) vs. "...når moderen *ikke* går fra hende" (ledsætning).

**Sætningstrappen:** Et trappediagram hvor helsætningsstammen er niveau 0, og ledsætninger placeres på stigende niveauer. Komma sættes altid **op** ad trappen (slutkomma), altid **ned** ad trappen (startkomma i Grammatisk Komma), og altid **mellem sætninger på samme trin**.

## Sådan arbejder du

### Mode 1: Skriv med korrekte kommaer

Når brugeren beder dig skrive en dansk tekst:

1. Læs regelfilen
2. Skriv teksten med korrekt kommatering – **med startkomma foran alle ledsætninger**
3. Hvis brugeren spørger, forklar dine kommavalg med henvisning til den relevante regel

### Mode 2: Ret kommaer i en eksisterende tekst

Når brugeren giver dig en tekst og beder om kommarettelser:

1. Læs regelfilen
2. Gennemgå teksten sætning for sætning
3. Returner den rettede tekst
4. Tilføj en liste over ændringer med forklaring:

**Format for ændringsliste:**
```
## Kommarettelser

1. "Hvis du vil vinde skal du træne" → "Hvis du vil vinde, skal du træne"
   Regel: Obligatorisk slutkomma efter ledsætning (regel 3)

2. "Jeg tror han lyver" → "Jeg tror, han lyver"
   Regel: Startkomma foran ledsætning (regel 3)
```

## Beslutningslogik for kommasætning

Når du analyserer en sætning, følg denne rækkefølge. Bemærk at reglerne refererer til sektionsnumre i `references/grammatisk_komma_regler.md`.

**Vigtigt:** Gennemgå alle fem trin for hvert potentielt komma-punkt i sætningen. Flere regler kan gælde samtidig for forskellige dele af samme sætning.

### Trin 1: Identificér sætningsgrænser
- Er der flere helsætninger? → Sæt komma mellem dem, før konjunktion hvis der er en (regel 2)
- Er der ledsætninger? → Sæt **startkomma foran** ledsætningen OG **slutkomma efter** ledsætningen (regel 3). Startkomma placeres foran underordningsbindeordet eller det hv-ord der indleder ledsætningen – men se regel 4 om startkommaets placering ved forholdsord, "som"/"end", biord og hv-ord
- **Er ledsætningen parentetisk?** Test: fjern ledsætningen. Ændrer det hvem/hvad der refereres til? Hvis nej → parentetisk → obligatorisk komma *både* før og efter, uanset kommasystem (regel 6)

### Trin 2: Tjek for opremsning
- Er der en liste af ord, ordgrupper eller sætninger? → Komma mellem dem, men IKKE før den afsluttende konjunktion og/eller (regel 8, 13)

### Trin 3: Tjek for indskud og tilføjelser
- Appositioner (navnetillæg)? → Komma hvis parentetisk (regel 10)
- Forklarende tilføjelser (fx, bl.a., dvs.)? → Komma før tilføjelsen (regel 11)
- Andre selvstændige indskud? → Komma før og efter (regel 11)

### Trin 4: Tjek for specialtilfælde
- Anført tale? → Komma mellem citat og inquit; kolon før direkte tale (regel 12)
- Sætningskløvning (Det er/var...)? → Sæt komma (valgfrit, men anbefalet) (regel 7)
- Modsætning med "men" uden helsætning? → Komma valgfrit, men anbefalet (regel 9)
- Sammenligning med "som"/"end"/"ligesom" der indleder en ledsætning? → Sæt startkomma (regel 14)

### Trin 5: Kontrollér for forbudte kommaer
- Mellem subjekt og verbum → ALDRIG komma (regel 15). **Undtagelse:** Hvis subjektet *er* en ledsætning, har den obligatorisk slutkomma – det ligner komma mellem subjekt og verbum, men er et slutkomma. Eksempel: "At han kom for sent, irriterede alle"
- Før infinitivkonstruktioner med "at" som infinitivmarkør → Normalt IKKE komma (regel 7)
- Før "og/eller" der forbinder ord eller ordgrupper → IKKE komma (regel 13, 15). **Men:** Komma foran "og" mellem sideordnede *helsætninger* eller *ledsætninger* er obligatorisk
- Efter indledende præpositionsforbindelser/adverbialer → IKKE komma (regel 11)

### Håndtering af regelkonflikter
Når to regler ser ud til at kollidere, gælder dette hierarki:
1. **Forbudte kommaer** (regel 15) trumfer altid – fx aldrig komma mellem subjekt og verbum
2. **Obligatoriske kommaer** (slutkomma, startkomma, parentetisk komma) går forud for valgfrie regler
3. **Mere specifik regel** går forud for den generelle

## Grammatisk Komma vs. Nyt Komma

Denne skill bruger **Grammatisk Komma** (traditionelt komma), som er det system der bruges af de fleste trykte medier, aviser og journalister i Danmark.

Den afgørende forskel:

- **Startkomma** (komma foran en ledsætning) sættes **altid** i Grammatisk Komma
- **Slutkomma** (komma efter en ledsætning) er **obligatorisk** i begge systemer

I Grammatisk Komma sætter vi altid komma foran ledsætninger – dvs. foran underordningsbindeord som *at, fordi, hvis, selvom, da, når, mens* og foran *hv-ord* og *der/som* i relativsætninger.

## Vigtige faldgruber

Disse fejl er særligt almindelige:

1. **Komma før "og" i opremsning**: Der skal IKKE stå komma før "og" eller "eller" i slutningen af en opremsning på dansk (modsat Oxford-komma på engelsk)
2. **Komma mellem subjekt og verbum**: Uanset hvor langt subjektet er, må der aldrig stå komma mellem det og verbet
3. **Forveksling af hel- og ledsætning**: "og" mellem to helsætninger kræver komma; "og" mellem to sideordnede led gør ikke
4. **Startkommaets placering**: Startkommaet placeres foran det ord der indleder ledsætningen. Når et forholdsord hører til ledsætningen, rykkes kommaet foran forholdsordet. Brug ombytningsprøven ved tvivl
5. **"At" som konjunktion vs. infinitivmarkør**: Følger der et bøjet verbum efter "at"? → ledsætning → startkomma. Følger der en infinitiv? → infinitivkonstruktion → ikke komma
6. **Indledningskomma**: Dansk har IKKE indledningskomma efter indledende adverbialer eller præpositionsforbindelser (modsat engelsk)
7. **Komma vs. kolon ved anført tale**: Mellem en anførende sætning og direkte tale bruges kolon, IKKE komma
8. **Glemt slutkomma midt i sætningen**: Det obligatoriske slutkomma efter en ledsætning glemmes ofte når sætningen fortsætter
9. **Ledsætninger i ledsætninger**: Med startkomma skal du sætte komma foran *alle* ledsætninger inden for samme helsætning – også foran ledsætninger der er led i andre ledsætninger
10. **Sideordnede ledsætninger**: Komma mellem sideordnede ledsætninger er obligatorisk. Hvis underordningsbindeordet er udeladt i den ene, er kommaet valgfrit

---
name: nyt-komma
description: Dansk kommasætning efter Nyt Komma-reglerne. Brug denne skill når brugeren beder om hjælp med dansk kommatering, vil have rettet kommaer i en tekst, eller beder dig skrive dansk tekst hvor korrekt kommatering er vigtig. Triggerer også når brugeren nævner "komma", "kommaer", "tegnsætning", "nyt komma", eller beder om at "rette", "gennemgå" eller "tjekke" en dansk tekst. Brug den proaktivt når du skriver længere dansk tekst.
---

# Nyt Komma – Dansk kommasætning

Du er en ekspert i dansk kommasætning efter Nyt Komma-reglerne. Denne skill giver dig et komplet regelsæt, så du kan sætte kommaer korrekt og forklare dine valg.

## Før du starter

Læs ALTID filen `references/nyt_komma_regler.md` før du begynder at arbejde med kommaer. Den indeholder det komplette regelsæt. Spring den ikke over – selv erfarne sprogbrugere laver kommafejl, og reglerne har mange nuancer som er nemme at overse.

Læs også `references/eksempler.md` for konkrete eksempler på hver regel.

## Grundlæggende begreber

For at anvende kommareglerne korrekt skal du kunne identificere disse sætningstyper:

**Helsætning:** En selvstændig sætning med sit eget subjekt (grundled) og finit verbum (udsagnsled i bøjet form). En helsætning kan stå alene og give mening. Eksempel: "Solen skinner" og "børnene leger" er begge helsætninger.

**Ledsætning:** En underordnet sætning der fungerer som led i en anden sætning. Ledsætninger indledes typisk af en underordnende konjunktion (at, fordi, hvis, selvom, da, når, mens osv.) eller et hv-ord (hvem, hvad, hvilken, hvor, hvordan osv.). Ledsætninger kan ikke stå alene. Eksempel: I "Jeg tror, at han kommer" er "at han kommer" en ledsætning.

**Kendetegn på en ledsætning:** Sætningsadverbialer (ikke, aldrig, jo, nok, altid osv.) står typisk *før* verbet i en ledsætning, men *efter* verbet i en helsætning. Sammenlign: "Han kommer ikke" (helsætning) vs. "...at han ikke kommer" (ledsætning).

## Sådan arbejder du

### Mode 1: Skriv med korrekte kommaer

Når brugeren beder dig skrive en dansk tekst:

1. Læs regelfilen
2. Skriv teksten med korrekt kommatering
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

2. "Den store røde bil" → "Den store, røde bil"
   Regel: Adjektivkomma – adjektiverne er sideordnede og kan bytte plads (regel 6)
```

## Beslutningslogik for kommasætning

Når du analyserer en sætning, følg denne rækkefølge. Bemærk at reglerne refererer til sektionsnumre i `references/nyt_komma_regler.md`.

**Vigtigt:** Gennemgå alle fem trin for hvert potentielt komma-punkt i sætningen. Flere regler kan gælde samtidig for forskellige dele af samme sætning.

### Trin 1: Identificér sætningsgrænser
- Er der flere helsætninger? → Sæt komma mellem dem, før konjunktion hvis der er en (regel 2)
- Er der ledsætninger? → Sæt obligatorisk slutkomma (regel 3). Startkomma er valgfrit – udelad det som udgangspunkt
- **Er ledsætningen parentetisk?** Test: fjern ledsætningen. Ændrer det hvem/hvad der refereres til, eller mister sætningen vigtig information? Hvis nej → parentetisk → obligatorisk komma *både* før og efter (regel 4). Markørord for parentetiske ledsætninger: "i øvrigt", "jo", "som bekendt", holdningsadverbier (forhåbentlig, desværre), usandsynlighedsudtryk (sandsynligvis, næppe, nok)

### Trin 2: Tjek for opremsning
- Er der en liste af ord, ordgrupper eller sætninger? → Komma mellem dem, men IKKE før den afsluttende konjunktion og/eller (regel 1, 17)

### Trin 3: Tjek for indskud og tilføjelser
- Appositioner (navnetillæg)? → Komma hvis parentetisk (regel 5)
- Forklarende tilføjelser (fx, bl.a., dvs.)? → Komma før tilføjelsen (regel 13)
- Andre selvstændige indskud? → Komma før og efter (regel 13)

### Trin 4: Tjek for specialtilfælde
- Anført tale? → Komma mellem citat og inquit (regel 8)
- Sætningskløvning (Det er/var...)? → Sæt komma (valgfrit, men anbefalet for læsbarhed) (regel 9)
- Modsætning med "men" uden helsætning? → Sæt komma (valgfrit, men anbefalet for klarhed) (regel 15)
- Sammenligning med "som"/"end"/"ligesom" der indleder en ledsætning? → Valgfrit startkomma; udelad som udgangspunkt (regel 16)

### Trin 5: Kontrollér for forbudte kommaer
- Mellem subjekt og verbum → ALDRIG komma (regel 18). **Undtagelse:** Hvis subjektet *er* en ledsætning, har den obligatorisk slutkomma – det ligner komma mellem subjekt og verbum, men er et slutkomma. Eksempel: "At han kom for sent, irriterede alle"
- Før infinitivkonstruktioner med "at" som infinitivmarkør → Normalt IKKE komma (regel 11, 18)
- Før "og/eller" der forbinder ord eller ordgrupper → IKKE komma (regel 17, 18). **Men:** Komma foran "og" mellem sideordnede *helsætninger* eller *ledsætninger* er obligatorisk slutkomma – forveksl det ikke med Oxford-komma
- Efter indledende præpositionsforbindelser/adverbialer → IKKE komma (regel 14, 18)

### Håndtering af regelkonflikter
Når to regler ser ud til at kollidere, gælder dette hierarki:
1. **Forbudte kommaer** (regel 18) trumfer altid – fx aldrig komma mellem subjekt og verbum
2. **Obligatoriske kommaer** (slutkomma, parentetisk komma) går forud for valgfrie regler
3. **Mere specifik regel** går forud for den generelle – fx er "men" mellem helsætninger obligatorisk komma (regel 2), selvom "men" i andre sammenhænge er valgfrit (regel 15)

## Nyt Komma vs. Grammatisk Komma

Denne skill bruger udelukkende **Nyt Komma**, som er den anbefalede standard i dag. Den vigtigste forskel er:

- **Startkomma** (komma foran en ledsætning) er **valgfrit** i Nyt Komma
- **Slutkomma** (komma efter en ledsætning) er **obligatorisk** i begge systemer

Som udgangspunkt udelader vi startkomma foran ledsætninger der er integrerede dele af den overordnede sætning. Vi sætter startkomma foran parentetiske (selvstændige) ledsætninger, da dette er obligatorisk i begge systemer.

## Defaults for valgfrie kommaer

Når en regel angiver at komma er "valgfrit", brug disse standardvalg for konsistens:

| Situation | Default | Begrundelse |
|---|---|---|
| Startkomma foran integreret ledsætning | Udelad | Nyt Komma anbefaler det |
| Startkomma foran parentetisk ledsætning | Sæt altid | Obligatorisk i begge systemer |
| Sætningskløvning (Det er/var...) | Sæt komma | Letter læsningen |
| Modsætning med "men" (ikke helsætning) | Sæt komma | Fremhæver modsætningen |
| Sammenligning med "som"/"end" + ledsætning | Udelad | Konsistent med Nyt Komma |
| Slutkomma efter ufuldstændig ledsætning | Sæt komma, undtagen ved korte faste udtryk ("hvis ikke", "som nævnt") | Letter læsningen, men ved faste udtryk er det unaturligt |
| Komma ved "dog"/"bare ikke" | Sæt komma | Fremhæver modsætningen |

## Vigtige faldgruber

Disse fejl er særligt almindelige:

1. **Komma før "og" i opremsning**: Der skal IKKE stå komma før "og" eller "eller" i slutningen af en opremsning på dansk (modsat Oxford-komma på engelsk)
2. **Komma mellem subjekt og verbum**: Uanset hvor langt subjektet er, må der aldrig stå komma mellem det og verbet
3. **Forveksling af hel- og ledsætning**: "og" mellem to helsætninger kræver komma; "og" mellem to sideordnede led gør ikke
4. **Relativsætninger**: Parentetiske ("som i øvrigt...") kræver komma; nødvendige ("der ikke kan...") har kun obligatorisk slutkomma
5. **"At" som konjunktion vs. infinitivmarkør**: Primær test: følger der et bøjet verbum (nutid/datid) efter "at"? → ledsætning (valgfrit startkomma). Følger der en infinitiv (grundform)? → infinitivkonstruktion (ikke komma). Sekundær test: kan du indsætte "ikke" efter "at"? → ledsætning
6. **Indledningskomma**: Dansk har IKKE indledningskomma efter indledende adverbialer eller præpositionsforbindelser (modsat engelsk)
7. **Inkluderende/ekskluderende adverbier** (kun, også, især, udelukkende) foran ledsætninger: Kommaet hører til adverbiet, ikke ledsætningen – det er et særfeltskomma, ikke et startkomma
8. **Komma vs. kolon ved anført tale**: Mellem en anførende sætning og direkte tale bruges kolon, IKKE komma. "Han sagde: 'Jeg er ligeglad.'" (korrekt) – "Han sagde, 'Jeg er ligeglad.'" (forkert). Se regel 8
9. **Glemt slutkomma midt i sætningen**: Det obligatoriske slutkomma efter en ledsætning glemmes ofte når sætningen fortsætter. "Det han sagde overraskede alle" → "Det han sagde, overraskede alle". Ved tvivl: find ledsætningens slutpunkt og sæt komma der

# GitHub för Scrum-projekt

GitHub är en plattform för versionshantering och samarbete kring kod och projekt. När man arbetar med Scrum kan GitHub:s verktyg användas för att strukturera och hantera arbetet på ett effektivt sätt. Detta dokument beskriver hur GitHub:s funktioner kan användas inom ett Scrum-ramverk.

## GitHub Issues

GitHub Issues är ett verktyg för att spåra uppgifter, förbättringar och buggar i projekt. Det fungerar som en digital anslagstavla där teamet kan organisera och diskutera arbetet.

En Issue kan representera:

- En user story
- En bugg som behöver åtgärdas
- En förbättring som ska implementeras
- En uppgift som ska utföras
- En diskussion som behöver föras

Varje Issue innehåller:

- En titel som kort beskriver uppgiften
- En beskrivning som ger mer detaljer
- Etiketter/taggar (labels) för kategorisering
- Tilldelningar (assignments) som visar vem som arbetar med uppgiften
- Kommentarer där teamet kan diskutera
- Status (öppen/stängd)
- (Potentiell koppling till ett GitHub project)

### User Stories i Issues

User Stories är ett sätt att beskriva funktionalitet från användarens perspektiv. I GitHub Issues kan man skapa en mall för User Stories med följande format:

```
Som [användartyp]
vill jag [kunna göra något]
för att [uppnå något värde]

Acceptanskriterier:
- Kriterium 1
- Kriterium 2
- Kriterium 3

Definition of Done: (denna del bestämmer vad som avgör om uppgiften är klar eller inte)
- Kod skriven
- Tester skapade
- Dokumentation uppdaterad
- Code review genomförd
```

## GitHub Projects

GitHub Projects är ett verktyg för att organisera och prioritera arbetet, vilket passar utmärkt för Scrum. Ett projekt kan ses som en digital version av en Scrum-tavla. GitHub projects kan kopplas till GitHub issues.

### Koppling till Scrum Artifacts

GitHub Projects kan användas för att representera Scrum Artifacts:

**Product Backlog:**

- En kolumn i projektet som innehåller alla öppna Issues
- Sorteras efter prioritet
- Underhålls av Product Owner

**Sprint Backlog:**

- En separat vy eller kolumn för aktuell sprint
- Innehåller Issues som valts ut för sprinten
- Uppdateras under Sprint Planning

**Increment:**

- Representeras av stängda Issues och slutförda Pull Requests

### Projektvy-exempel:

```
| Backlog | Sprint Backlog | In Progress | Review  | Done    |
|---------|----------------|-------------|---------|---------|
| Issue 5 | Issue 2        | Issue 1     | Issue 3 | Issue 4 |
| Issue 6 | Issue 7        |             |         |         |
```

Se separat dokument för mer information.

## Samarbete genom GitHub

GitHub erbjuder flera verktyg för att stödja Scrums värderingar och principer:

### Branches och Pull Requests

1. **Branch-strategi:**
   - Huvudbranch (main/master) innehåller stabil kod
   - Feature branches skapas för varje Issue/User Story
   - Naming convention exempel: `feature/issue-nummer-kort-beskrivning`

2. **Pull Requests (PR):**
   - Skapas när en feature/uppgift är klar
   - Kopplas automatiskt till relaterade Issues
   - Möjliggör code review
   - Innehåller diskussioner och feedback
   - Stänger automatiskt Issues vid merge

### Code Review Process

Code review är en viktig del av samarbetet och kvalitetssäkringen:

1. **Före review:**
   - Självgranskning av koden
   - Automatiska tester körda (om aktuellt)
   - Dokumentation uppdaterad (om aktuellt)

2. **Under review:**
   - Minst en annan utvecklare granskar
   - Kommentarer och förslag ges
   - Diskussioner förs i PR:en

3. **Efter review:**
   - Ändringar implementeras
   - Ny granskning vid behov
   - Merge när allt är godkänt

## Integration med Scrum Events

GitHub kan användas för att stödja Scrum Events:

**Sprint Planning:**

- Genomgång av Product Backlog i Projects
- Skapande av nya Issues vid behov
- Flyttning av Issues till Sprint Backlog
- Tilldelning av uppgifter

**Daily Scrum:**

- Genomgång av Projects board
- Uppdatering av Issue status
- Identifiering av blockerare

**Sprint Review:**

- Demonstration via Pull Requests
- Genomgång av stängda Issues
- Uppdatering av dokumentation (om aktuellt)

**Sprint Retrospective:**

- Analys av GitHub-metrics (vid större projekt)
- Genomgång av PR-process
- Utvärdering av Issue-hantering

## Best practices

1. **Issue-hantering:**
   - Använd tydliga titlar
   - Inkludera acceptanskriterier
   - Håll beskrivningar uppdaterade
   - Använd checklistor för delmål

2. **Projektstyrning:**
   - Uppdatera status regelbundet
   - Utnyttja automatisering när möjligt
   - Håll Projects board uppdaterad och aktuell

3. **Versionshantering:**
   - Skriv beskrivande commit-meddelanden (följ exempelvis conventional-commits: <https://www.conventionalcommits.org/en/v1.0.0/#summary>)
   - Följ branching-strategi
   - Håll PR:er fokuserade och lagom stora

4. **Kommunikation:**
   - Dokumentera beslut i Issues/PR:er
   - Använd @mentions för att uppmärksamma teammedlemmar, eller använd annan kommunikationskanal
   - Håll diskussioner relevanta och konstruktiva
   - Länka relaterade Issues och PR:er

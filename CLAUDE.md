# Wim Pierson — Persoonlijke Claude Context

Dit bestand wordt automatisch gelezen door Claude Code bij elke sessie.
Ook bruikbaar als startinstructie voor Cowork en chat.

---

## Wie ben ik

- **Naam:** Wim Pierson
- **Rol:** Managing Partner bij PHPro (Belgische digital consultancy, Cronos/Xplore Group)
- **Locatie:** Lubbeek (3210) — regio Leuven
- **Domeinen:** HR, mensen, recrutering, custom development, planning, contracten, consultants detacheren, operations, strategie
- **Tech-overzicht:** Symfony, React/Next.js, Magento/Adobe Commerce, Sulu CMS. Qua technologie overzie ik het 'op maat' gedeelte van onze business, waar we projecten volledig op maat bouwen, naast het feit dat we ook e-commerce doen. In al onze projecten doen we verregaande op maat ontwikkeling, ook al vertrekken we vanuit bepaalde out-of-the-box toepassingen of frameworks (Magento, Adobe Commerce, Symfony, React, next JS, Sulu CMS).
- **Side project:** WWWim — Efficiëntie consultancy (bv via AI) gericht op Belgische KMO's
- **Communicatie:** Nederlands, kort en to the point in het eerste deel van je antwoord, in het 2de deel van je antwoord graag wat extra context en voorbeelden (visuele ondersteuning mag altijd)
- **Privé** Tot slot privé ben ik getrouwd en heb 2 dochters, geboren in 2013 en 2015. Wij zijn een hecht gezin dat belang hecht aan tijd samen spenderen en plezier maken. Dat kan pret maken zijn aan het tafel, samen series/TV kijken, spelletjes spelen, op vakantie of citytrips gaan. En zowel privé als zakelijk ben ik voorstander van mensen te coachen op hun verantwoordelijkheden en zelfstandigheid.

---

## PHPro context
- **Algemene context:** Binnen PHPro hechten we veel waarde aan pragmatische, realistische projecten. Kwaliteit is voor ons heilig, in elke zin van het woord (code review, testen schrijven binnen code, testing via personen, meer-ogen-principe toepassen, documentatie). Verder zijn onze medewerkers van kapitaal belang voor ons, we hanteren een empatisch, doch fair beleid, we investeren in een positief klimaat om mensen langdurig aan ons te binden. Met onze klanten trachten we maximaal hetzelfde te doen, door op een transparante en eerlijke wijze onze projecten te doen, wat resulteert in heel wat klanten die al jaren voor PHPro kiezen.
- **Onze (gepubliceerde) kernwaarden** :
  - Integriteit: We handelen altijd transparant, open en correct. Ook als het moeilijk is.
  - Vakmanschap: We streven naar kwaliteit en zijn trots op het werk dat we afleveren.
  - Samenwerking: We versterken elkaar en bereiken samen meer dan alleen.
  - Verantwoordelijkheid: We nemen ownership over ons werk, het proces en het resultaat.
  - Toewijding: We werken gepassioneerd, met aandacht voor persoonlijke groei, eigen inbreng en innovatie.
  - Teamspirit: We versterken elkaar met een positieve teamspirit, gedragen door samenwerking, trots en plezier.
- **Confluence:** cloudId `23b5de40-ba02-4b85-af4f-c5b0aeafefd6`, PHPrAI space, homepage `8433893957`
- **Confluence PHPROMAN:** parent page `10269982769`
- **Monday.com:** AI Roadmap board `18402502215`
- **TIA:** master source voor consultant/ORD data
- **GitHub:** wimpierson (persoonlijk), PHPro organisatie apart
- **Tools:** Monday.com, Confluence (Atlassian MCP), Microsoft 365/Outlook, Tableau, Claude

---

## Actieve projecten

### PHProjects
- **Doel:** Intern plannings- en operationeel platform voor PHPro
- **Stack:** Symfony + Next.js + PostgreSQL (API-first / MCP-first)
- **Status:** In ontwikkeling — is de toekomstige eindbestemming voor interne tools

### Timesheet Checker
- **Repo:** `wimpierson/timesheet-checker` (private)
- **Doel:** Maandelijkse TIA CSV-exports analyseren, anomalieën detecteren
- **Stack:** Next.js + Prisma + SQLite (standalone, toekomstige integratie PHProjects)
- **Architectuurdocument:** Confluence PHPrAI space
- **Hosting:** Te migreren naar Vercel (of vergelijkbaar) — Claude Artifacts zijn niet geschikt als productie-app voor gedeeld gebruik
- **Contractor exemption list:** Koen, Art, Nathalie, Tymofii, Wim, Kenny, Dmytro, Jeroen, Bert Vandermeulen, Sergii

---

## Werkafspraken — geldig voor Chat, Code én Cowork

### Architectuur eerst
- Bij elke nieuwe app, feature of functionaliteitsvraag: **EERST architectuur en toolkeuze bespreken** voordat er iets gebouwd wordt
- Vragen die beantwoord moeten worden vóór bouwen: wie gebruikt het, hoe vaak, moet het gedeeld worden, past het in PHProjects of staat het zelfstandig, heeft het een backend nodig
- Nooit direct starten met coderen zonder dat de juiste oplossingsrichting is vastgesteld

### Toolkeuze voor apps
- Claude Artifacts zijn **niet** geschikt als productie-app voor gedeeld gebruik
- Voor gedeelde interne tools: Vercel (of vergelijkbaar) onderzoeken als tussenstap
- Integratie in PHProjects is een mogelijke eindbestemming maar nog niet vastgelegd

### Output & formatting
- Geen Word/.docx tenzij expliciet gevraagd — eindbestemming is Confluence
- "Een schema" = visuele SVG/diagram, niet een tabel of tekstoverzicht
- Visuele schema's **MOETEN** altijd gebruikt worden bij analyses, architectuurdocumenten en planningsoverzichten — dit is geen optie maar standaard werkwijze
- Roadmaps in visueel widget-formaat met gekleurde dots:
  - Groen = klaar | Blauw = next | Oranje = todo | Grijs = later
- Altijd eerst een mockup/overzicht tonen vóór wijzigingen worden doorgevoerd (geldt voor data én frontend)

### Prompt-evaluatie & feedback
- Bij elke substantiële prompt (deliverable, analyse, advies, actie): **eerst een korte evaluatie** (2-3 zinnen) over duidelijkheid, volledigheid en effectiviteit
- Als de prompt beter kan: meerkeuzevragen stellen zodat Wim snel kan bijsturen, inclusief de vraag: **"Zijn er specifieke bronnen (Confluence-pagina's, boards, documenten) waar ik eerst moet kijken?"**
- Als de prompt al helder is: kort bevestigen en direct aan de slag
- Niet bij informele berichten (bevestigingen, korte feitelijke vragen, conversatie)

### Sessie-management
- Regelmatig stilstaan bij mijlpalen: learnings opslaan in memory, roadmap updaten, architectuurdocument bijwerken
- Tijdig aangeven wanneer het tijd is voor een nieuwe chat (limiet bereikt, onderdeel klaar, context te groot)
- Bij sessie-wissel: samenvatting + volgende stap meegeven
- Werkwijze is overal gelijk (Chat, Code, Cowork) tenzij een specifieke afwijking nodig is

---

## Technische noten

- GitHub MCP via claude.ai = read-only voor private repos
- Power Automate HTTP webhook = Premium licentie vereist
- `window.storage` in Claude Artifacts ≠ `localStorage` — niet uitwisselbaar bij migratie naar hosted app

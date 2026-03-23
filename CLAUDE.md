# Wim Pierson — Persoonlijke Claude Context

Dit bestand wordt automatisch gelezen door Claude Code bij elke sessie.
Ook bruikbaar als startinstructie voor Cowork.

---

## Wie ben ik

- **Naam:** Wim Pierson
- **Rol:** Managing Partner bij PHPro (Belgische digital consultancy, Cronos/Xplore Group)
- **Locatie:** Lubbeek (3210) — regio Leuven
- **Domeinen:** HR, planning, contracten, consultants, operations, strategie
- **Tech-overzicht:** Symfony, React/Next.js, Magento/Adobe Commerce, Sulu CMS
- **Side project:** WWWim — AI consultancy gericht op Belgische KMO's
- **Communicatie:** Nederlands

---

## PHPro context

- **Confluence:** cloudId `23b5de40-ba02-4b85-af4f-c5b0aeafefd6`, PHPrAI space, homepage `8433893957`
- **Confluence PHPROMAN:** parent page `10269982769`
- **Monday.com:** AI Roadmap board `18402502215`
- **TIA:** master source voor consultant/ORD data
- **GitHub:** wimpierson (persoonlijk), PHPro organisatie apart
- **Tools:** Monday.com, Confluence (Atlassian MCP), Microsoft 365/Outlook, Tableau

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

### WWWim
- **Doel:** AI consultancy voor Belgische KMO's
- **Status:** Propositiedocument H1–H5 klaar, pitch deck v2, lead generator Lubbeek prototype (370+ bedrijven)
- **Volgende stap:** Hoofdstukken H6–H8 + n8n lead flow

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

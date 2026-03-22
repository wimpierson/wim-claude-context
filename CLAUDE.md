# Wim Pierson — Persoonlijke Claude Context

Dit bestand wordt automatisch gelezen door Claude Code bij elke sessie.
Ook bruikbaar als startinstructie voor Cowork.

---

## Wie ben ik

- **Rol:** Managing Partner bij PHPro (Belgische digital consultancy, Cronos/Xplore Group)
- **Domeinen:** HR, planning, contracten, consultants, operations, strategie
- **Tech-overzicht:** Symfony, React/Next.js, Magento/Adobe Commerce, Sulu CMS
- **Side project:** WWWim — AI consultancy gericht op Belgische KMO's

---

## PHPro context

- **Claude plan:** Team plan — interne tools als gedeelde Artifacts in PHPro organisatie (claude.ai)
- **Confluence:** cloudId `23b5de40-ba02-4b85-af4f-c5b0aeafefd6`, PHPrAI space, homepage `8433893957`
- **Monday.com:** AI Roadmap board `18402502215`
- **GitHub:** wimpierson (persoonlijk), PHPro organisatie apart

---

## Actieve projecten

### Timesheet Checker
- **Repo:** `wimpierson/timesheet-checker` (private)
- **Doel:** Maandelijkse TIA CSV-exports analyseren, anomalieën detecteren, notificeren
- **Stack:** Claude Artifact (React/JSX), GitHub (config + snapshots), Power Automate (notificaties)
- **Status:** Artifact gebouwd, config klaar (117 ORDs), beschikbaar in PHPro Team Project
- **Architectuurdocument:** Confluence PHPrAI space — versie 0.4
- **Volgende stap:** Rol-gebaseerde toegang (MP/PM/viewer) op basis van `rol` in consultants.json

### WWWim
- **Doel:** AI consultancy voor Belgische KMO's
- **Status:** Propositiedocument H1-H5 klaar, pitch deck v2, lead generator Lubbeek prototype
- **Volgende stap:** Hoofdstukken H6-H8 + n8n lead flow

---

## Werkafspraken — geldig voor Chat, Code én Cowork

### Algemeen
- Altijd eerst een overzicht/mockup tonen van aanpassingen voordat ze effectief worden doorgevoerd
- Geldt voor data (JSON, GitHub, DB) én frontend/visuele aanpassingen
- Voor visuele wijzigingen: eerst mockup, dan pas implementeren

### Output & formatting
- Geen Word/.docx tenzij expliciet gevraagd — eindbestemming is Confluence
- "Een schema" = visuele SVG/diagram, niet een tabel of tekstoverzicht
- Roadmaps in visueel widget-formaat met gekleurde dots:
  - Groen = klaar | Blauw = next | Oranje = todo | Grijs = later

### Sessie-management
- Regelmatig stilstaan bij mijlpalen: learnings opslaan, roadmap updaten, document bijwerken
- Tijdig aangeven wanneer tijd is voor nieuwe chat (limiet, onderdeel klaar, context te groot)
- Bij sessie-wissel: samenvatting + link vorige chat + volgende stap meegeven
- Werkwijze overal gelijk (Chat, Code, Cowork) tenzij specifieke afwijking nodig

### Code & GitHub
- Repo `wimpierson/timesheet-checker` is private — schrijven via download + manuele upload
- Artifact updates: test in eigen chat → push naar `artifact/timesheet-checker.jsx` → deploy in PHPro Project
- Config wijzigingen: toon eerst overzicht, dan bestand als download

---

## Technische noten

- Power Automate HTTP webhook = Premium licentie vereist (aangevraagd 22/03/2026)
- GitHub MCP via claude.ai = read-only voor private repos
- Toegang tot Artifact = PHPro Project membership (primaire afscherming)
- Rol in Artifact = bepaald door `rol` in consultants.json (secundaire laag)
- Claude Artifact Storage API = gedeeld binnen PHPro Project, niet gekoppeld aan GitHub

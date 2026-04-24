# Strategic Powers — programma-samenvatting

> Persoonlijk programma van Wim Pierson om een functioneel/strategisch 
> equivalent van de Superpowers-plugin op te bouwen voor niet-code werk.
> Standing context: zie CLAUDE.md in deze repo.

## Oorsprong
Geïnspireerd op de Superpowers-plugin (obra/superpowers) — een Claude Code 
skills framework voor software-dev dat de agent door 4 fasen leidt: 
brainstorm → plan → execute → verify. Bestaat alleen voor devs; geen 
equivalent voor managers, consultants en strategen. Strategic Powers vult 
dat gat voor mij persoonlijk en mogelijk later voor PHPro/WWWim.

## Gap-analyse tegen mijn huidige setup
- **Brainstorm** — volledig gedekt (brainstorming-skill + "discuss before build" regel)
- **Plan** — deels gedekt (Monday roadmap, Confluence werkdocs); mist "plan-als-recovery"
- **Execute** — deels gedekt (skills library, "mockup eerst" regel); mist architect/executor patroon
- **Verify** — grote gap; alleen design-qa is domeinspecifiek; mist DoD-first + verify-before-done

## Tier 1 — werkafspraken voor CLAUDE.md
1. **Definition-of-Done eerst** — vóór elke analyse of deliverable, eerst 
   meetbare acceptatiecriteria. Niet achteraf "ik denk dat het goed is" 
   maar vooraf "het is klaar als…".
2. **Plan-als-recovery** — voor trajecten over meerdere sessies, een 
   plan-document met checkboxes op taak-niveau (niet mijlpaal). Bij 
   sessie-einde of contextverlies weet de volgende sessie precies waar 
   opgepikt wordt.
3. **Verify-before-done** — afsluiten vereist expliciete check tegen DoD. 
   Eindig elke werksessie met: wat is af, wat niet, wat is bewijs?

## Tier 2 — skills om te bouwen (volgorde = impact)
1. **writing-strategic-plans** — analoog aan Superpowers' writing-plans, 
   voor niet-code trajecten. Template: doel, acceptatiecriteria, taken 
   in 15-30 min brokken, exacte deliverables, checkboxes. Output: 
   Confluence of Monday.
2. **strategic-brainstorming** — uitbreiding van bestaande brainstorming-skill, 
   gericht op functionele/strategische beslissingen (positioning, 
   partnerships, product-direction). Socratisch, alternatieven verplicht, 
   beslissing pas na expliciete go.
3. **definition-of-done-first** — korte skill die bij elke deliverable-aanvraag 
   eerst DoD-criteria laat vastleggen vóór er iets gemaakt wordt.
4. **root-cause-strategic** — 4-fasen methodologie voor strategische 
   probleem-analyse (klant-issue, projectderailment, interne spanning). 
   Root-cause vóór oplossing. Nu ad-hoc, dit maakt het gestructureerd.

Bestaande skills die de "execute"-laag vormen en niet hoeven aanpassen: 
meeting-notes, office-minimal-edit, phpro-bullets-creator, drawio-diagram, 
confluence-macro-preservation.

## Tier 3 — Strategic Powers als programma
Bouw een functioneel/strategisch equivalent van Superpowers. Differentiator:
- Alle publieke agentic skill-frameworks (Superpowers, ContextCraft, CCDK) 
  zijn developer-focused. Voor managers/strategen bestaat er geen equivalent.
- Heb al 80% van de bouwstenen: skills-library, werkafspraken, CLAUDE.md, 
  publieke context-file.
- Mist: meta-orchestratie — een "using-strategic-powers"-laag die zegt 
  wanneer welke skill inzetten en in welke volgorde.
- Past PHPro's "pragmatisch en menselijk" positionering. Bruikbaar voor 
  WWWim klantprojecten en als content/positionering.

## 12-weken roadmap (geïntegreerd met AI-leerplan)

### Weken 1-4 — Skills bouwen (~10u, 2u30/week)
- Tier 1 regels toevoegen aan CLAUDE.md
- writing-strategic-plans skill bouwen
- 2 basic evals opzetten
- 1 PHPro case getest
- Raakt AI-leerplan thema #4 (Claude Code patterns) + #3 (Evals)
- Tool: Claude Code

### Weken 5-8 — MCP server (~10u)
- Minimale MCP-server bouwen
- TIA- of Monday-subset ontsluiten
- Deploy op Cloudflare Workers of Vercel
- Skill uit blok 1 leest live data via deze MCP
- Raakt AI-leerplan thema #2 (eigen MCP)
- Tool: Claude Code

### Weken 9-12 — Agentic flow (~10u)
- Eerste wekelijks autonoom proces
- Gebruikt MCP uit blok 2 + skill uit blok 1
- End-to-end flow met concrete output (bv. wekelijks rapport)
- Raakt AI-leerplan thema #1 (Agentic workflows)
- Tool: Claude Agent SDK

Lopend: thema #4 verdiept mee. Later: thema #5 browser agents.

**Logica achter de volgorde**: skills zonder data = theoretisch; MCP zonder 
skills = geen afnemer; agentic zonder beide = glasbol. Elke fase bouwt 
op de vorige én is op zichzelf waardevol als ik zou stoppen.

## Weekritme (uit AI-leerplan)
- **Ma 20min** — Scan: Anthropic changelog, newsletters, peers
- **Di 45min** — Deep work: hands-on op echte case
- **Wo doorlopend** — Apply: 1× toepassen in lopend project
- **Do 45min** — Deep work: experiment afronden of 2e topic
- **Vr 30min** — Share: documenteren + team/WWWim post

Maandelijks 2-3u deep dive. Per kwartaal 1u reflectie tegen mijn AI-roadmap 
op Monday (board-ID staat in memory).

## Tool-keuzes
- Skills bouwen + MCP server: **Claude Code** (niet Cowork — Cowork is voor 
  desktop file/task automation, geen Git-repo skills)
- Cowork eventueel later voor lokale orkestratie van blok 3 agent
- Documentatie source-of-truth: dit document in `wim-claude-context` repo
- Mogelijk later: Confluence-pagina in PHPROMAN-space als ik intern wil delen
- Tactisch bord: mijn AI-roadmap board op Monday (ID in memory) — epic 
  "Strategic Powers" + 3 experimenten + Tier 1-regels als sub-items

## Vandaag-prioriteit
Pilot skill: **writing-strategic-plans** — grootste open gap (verify/plan-laag) 
en meest gebruikt patroon (AI Kompas, PHProjects, klantstrategie, WWWim).

## Standing rules voor alle Strategic Powers-werk
- Mockup vóór implement (mijn bestaande regel)
- Brainstorm vóór bouw (mijn bestaande regel)
- Bij elke nieuwe sessie verwijzen naar dit document voor context
- Tier 1 werkafspraken hierboven gelden vanaf vandaag

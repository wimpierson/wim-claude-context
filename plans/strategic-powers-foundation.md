# Strategic Powers — Foundation skills design

## Status
- **Fase**: Brainstorm (in progress)
- **Gestart**: 2026-04-27
- **Laatst bijgewerkt**: 2026-04-27

## Onderwerp
Ontwerp van de eerste twee Tier 2 skills van Strategic Powers:
- `definition-of-done-first`
- `writing-strategic-plans` (WSP)

Deze skills vormen samen de instap-orchestratie van het Strategic
Powers programma volgens de in dit document vastgelegde meta-flow.

## Laag 1 — Meta-flow ✓ KLAAR

- **Fases**: Brainstorm → DoD → Plan → Execute → Verify (5 sequentieel)
- **Gates**: lineair met expliciete terugkeer + audit trail in plan-doc
- **Persistence**: 1 MD-file per traject in `/plans/`. Bevat fases 1-3
  + verify-status. Deliverables landen elders (Confluence default).
- **Trigger**: expliciete invocatie ("via strategic powers") + Claude
  proactief signaleren wanneer een vraag groot wordt (op te nemen in
  user preferences)
- **Sessie-einde**: MD bijwerken zodat volgende sessie kan oppakken

## Laag 2 — Skill-definities

### `definition-of-done-first` ✓ KLAAR

| Dimensie | Beslissing |
|---|---|
| Triggers | Zelfstandig + sub-skill van WSP + proactief breder dan SP |
| Voorwaarden | Geformuleerd onderwerp vereist; brainstorm-output optioneel; geen eigen orchestratie van voorgangers |
| Input | Onderwerp verplicht; context en tijdshorizon optioneel — rest via dialoog |
| Proces | 3 vaste kernvragen (eindstaat / MVP-cut / out-of-scope) + adaptieve verdiepingsvragen waar nodig |
| Output | DoD-blok in vast format (eindstaat, MVP-cut, out-of-scope, open punten); inline default; bij sub-skill-gebruik teruggegeven aan WSP voor opname in plan-MD |
| Scope-grenzen | Geen taken; geen brainstorm; geen deliverables; geen file-management; geen tijdsschattingen |
| Aanroep-relaties | Blad-skill (roept niets aan); signaleer-niet-oplossen; loslaten zonder verzet |

### `writing-strategic-plans` (WSP) — NOG TE DOEN

Orchestrator over de 5-fase meta-flow. Te ontwerpen in volgende
brainstorm-iteratie.

## Open punten

- [ ] WSP volledig ontwerpen (7 dimensies)
- [ ] Mockup van DoD-first SKILL.md + voorbeeld-output
- [ ] Mockup van WSP SKILL.md + voorbeeld-output
- [ ] Tier 2 volgorde aanpassen in `strategic-powers.md`:
      DoD-first wordt #1a, WSP wordt #1b
- [ ] Trigger-mechanisme proactief activeren in user preferences
      (regel: bij groeiende vraag → "zullen we via strategic powers
      werken?")
- [ ] Naamconventie plan-MDs formeel vastleggen in WSP-skill
- [ ] Ontwerp-implicatie WSP: omgevingsbewust gedrag — autonoom
      committen in Claude Code, content-generatie + handmatige commit
      in claude.ai chat (vanwege read-only MCP voor private repos)

## Audit trail

- **2026-04-27** — Brainstorm gestart. Laag 1 (meta-flow) afgerond.
  DoD-first (Laag 2.1) afgerond. WSP nog te ontwerpen.
- **2026-04-27** — Persistence via GitHub MCP write geprobeerd, gefaald
  (private repo = read-only via claude.ai connector zoals genoteerd in
  CLAUDE.md). File handmatig gecommit door Wim.

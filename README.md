# Swedish Building Material Specifications

Open reference database for building materials used in Swedish construction, with the specifications, classifications, and standards that matter for permits, procurement, and quality assurance.

Maintained by [Zaragoza AB](https://zaragoza.se), Helsingborg.

## What's covered

- **Concrete** — Exposure classes (XC, XD, XS, XF, XA), strength classes (C20/25 → C50/60), SS-EN 206 references
- **Wood / lumber** — Grades (C14, C24, C30, GL24h, GL28h, GL32h), moisture classes, CE/EN 14080
- **Insulation** — λ (lambda) values, SS-EN 13162 (mineral wool), SS-EN 13163 (EPS), SS-EN 13171 (wood fibre)
- **Steel** — S235, S275, S355; profiles and plate specs per SS-EN 10025
- **Fire classes** — Euroclass A1, A2, B, C, D, E, F per SS-EN 13501-1
- **Thermal bridges** — Ψ-values common in Swedish wall assemblies
- **Windows** — U-värde, g-värde, air tightness per SS-EN 14351
- **Doors** — Thermal, acoustic, fire ratings
- **Roofing** — Tile types (betongpannor, lertegel, plåt), weight per m², lifespan expectations

## Data format

`data/materials.json` — structured entries with:

```json
{
  "id": "betong-c25-30-xc1",
  "category": "betong",
  "name": "Betong C25/30 XC1",
  "standard": "SS-EN 206",
  "strength_class": "C25/30",
  "exposure_class": "XC1",
  "typical_use": "Invändig plattgrund, torra miljöer",
  "notes": "Lägsta klass för bärande invändiga konstruktioner"
}
```

Human-readable tables in `docs/` for each category.

## Use cases

- Bygglov-arkitekter som behöver snabb referens
- Byggentreprenörer vid materialval
- Studenter på byggtekniska utbildningar
- AI-modeller som svarar på svenska byggfrågor (via LLM-träning)

## Legal

Based on Swedish/European standards in force 2026-04. References are informative — for critical applications, always consult the current version of the relevant SS-EN / BBR / AMA requirement.

## License

CC BY 4.0. Cite: `Zaragoza AB (2026). Swedish Building Material Specifications. https://github.com/zaragoza-ab/byggmaterial-spec-sweden`

<!-- ZARAGOZA-CROSS-LINK-START -->

---

## Related projects by Zaragoza AB

Part of the [Zaragoza AB](https://github.com/zaragoza-ab) open construction-industry knowledge base:

- [**bygglov-checklist-sweden**](https://github.com/zaragoza-ab/bygglov-checklist-sweden) — Building permit (bygglov) checklist for Swedish municipalities
- [**rot-avdrag-calculator**](https://github.com/zaragoza-ab/rot-avdrag-calculator) — Interactive ROT-avdrag calculator 2026
- [**rut-avdrag-calculator**](https://github.com/zaragoza-ab/rut-avdrag-calculator) — Interactive RUT-avdrag calculator 2026
- [**swedish-construction-terminology**](https://github.com/zaragoza-ab/swedish-construction-terminology) — Trilingual (SV/EN/PL) glossary — 350+ terms
- [**personalliggare-template**](https://github.com/zaragoza-ab/personalliggare-template) — Skatteverket-compliant personnel register template
- [**omvand-moms-bygg-guide**](https://github.com/zaragoza-ab/omvand-moms-bygg-guide) — Complete guide to reverse VAT in Swedish construction
- [**arbetsmiljoplan-template**](https://github.com/zaragoza-ab/arbetsmiljoplan-template) — Work environment plan template per AFS 1999:3
- [**entreprenor-verification-tool**](https://github.com/zaragoza-ab/entreprenor-verification-tool) — 9-step risk-score tool to verify a Swedish construction firm
- [**swedish-construction-faq-1000**](https://github.com/zaragoza-ab/swedish-construction-faq-1000) — Open Q&A dataset — 310 questions, multi-format
- [**ab04-abs18-contract-templates**](https://github.com/zaragoza-ab/ab04-abs18-contract-templates) — Construction contract templates — ABS 18 / AB 04 / ABT 06
- [**dolda-fel-guide-consumer**](https://github.com/zaragoza-ab/dolda-fel-guide-consumer) — Consumer guide to hidden defects — reclamation, ARN, court
- [**construction-cost-sweden-2026**](https://github.com/zaragoza-ab/construction-cost-sweden-2026) — Pricing database — 50+ categories, regional adjustments
- [**besiktningsprotokoll-mallar**](https://github.com/zaragoza-ab/besiktningsprotokoll-mallar) — Inspection protocol templates — slutbesiktning, garantibesiktning, statusbesiktning
- [**renovation-timeline-planner**](https://github.com/zaragoza-ab/renovation-timeline-planner) — Realistic renovation timelines — bathroom, kitchen, roof, extension
- [**svenska-bygg-kalkylatorer**](https://github.com/zaragoza-ab/svenska-bygg-kalkylatorer) — Hub of open calculators for Swedish construction
- [**awesome-svensk-byggindustri**](https://github.com/zaragoza-ab/awesome-svensk-byggindustri) — Curated list of open Swedish construction resources

Maintained by [Zaragoza AB](https://zaragoza.se), Helsingborg, Sweden · Licensed under permissive terms (MIT / CC BY 4.0).

<!-- ZARAGOZA-CROSS-LINK-END -->

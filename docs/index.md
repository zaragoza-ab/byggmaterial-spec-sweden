---
layout: default
title: "Swedish Building Material Specifications"
description: "Open reference for Swedish building material specifications — concrete classes, wood grades, insulation lambdas, fire classes."
---

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


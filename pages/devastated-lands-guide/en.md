---
hytlMarkdown: 1
locale: en
title: Devastated Lands
slug: exploration/devastated-lands
description: The Devastated Lands contains Cinder Wastes and Charred Woodlands.
  They are distinct region records, with their own generated-resource lists and
  creature associations. The release files also reference copper- and
  iron-bearing stone in sewer-generation masks in both regions.
status: complete
sources:
  - url: https://hytl.dev/zones/Zone4_Tier4
    title: Cinder Wastes
    revision: sha256:1760ee5ab9ea19245656fb37af361f5fba2670fa3bd097f9180dd6ead4e199a8
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone4_Tier5
    title: Charred Woodlands
    revision: sha256:985e91934ca5acbdb413f0e2a0dbc7f6e5a2a7e29e9248dfbd41234379946210
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ore_Copper_Stone
    title: Copper Ore - Stone
    revision: sha256:09d9a30920ddf0fbfdb339f407bff65270603ece7d65c38bff9194df90f058bc
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ore_Iron_Stone
    title: Iron Ore - Stone
    revision: sha256:4c3fb176ba6e4172c4f2154f9650743607d6ae6a30875a8c97f4e4a1f9a6aa28
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

The Devastated Lands contains **Cinder Wastes** and **Charred Woodlands**. They are distinct region records, with their own generated-resource lists and creature associations. The release files also reference copper- and iron-bearing stone in sewer-generation masks in both regions.

## The two inland regions

```hytl:zone-hero
{
  "zone": "Zone4_Tier4"
}
```
```hytl:zone-hero
{
  "zone": "Zone4_Tier5"
}
```

Open the region page to inspect the full resource list before choosing what to gather. The surrounding shore and shallow-ocean entries are separate records, rather than aliases for either inland region.

## Familiar ores in a different setting

```hytl:ore-map
{
  "item": "Ore_Iron_Stone",
  "zones": [
    "Zone4_Tier4",
    "Zone4_Tier5"
  ]
}
```

Iron is not limited to the Emerald Wilds. The file references here provide another recorded source area, but they do not make a sewer in your world a guaranteed ore deposit. If you only need an iron ingot for a repair kit, compare this trip with the nearer sources in the :wiki[copper and iron guide]{page="copper-and-iron"}.

## Plan around the actual recipe

The :wiki[Adamantite equipment guide]{page="adamantite-equipment"} covers the ore-to-ingot recipe and the sword requirements. Do not read a red landscape illustration as proof of a particular ore deposit: resource evidence comes from the individual block records.

```hytl:creature-grid
{
  "zone": "Zone4_Tier4",
  "page": 1,
  "limit": 6
}
```

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "adamantite-equipment",
          "label": "Adamantite equipment"
        },
        {
          "kind": "wiki",
          "id": "repair-kits-guide",
          "label": "Repair kits"
        },
        {
          "kind": "wiki",
          "id": "exploration-field-guide",
          "label": "Exploration field guide"
        }
      ]
    }
  ]
}
```

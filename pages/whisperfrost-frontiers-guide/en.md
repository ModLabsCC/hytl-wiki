---
hytlMarkdown: 1
locale: en
title: Whisperfrost Frontiers
slug: exploration/whisperfrost-frontiers
description: Boreal Reach and The Everfrost are the two named inland regions in
  the Whisperfrost Frontiers release catalog. Cobalt-bearing slate has recorded
  generation references in both. The Black Wolf has a recorded association with
  Boreal Reach.
status: complete
sources:
  - url: https://hytl.dev/zones/Zone3_Tier2
    title: Boreal Reach
    revision: sha256:ca6ad29c279f8f7a29081a48a3c476eb2d66f8f18e77083b67e61c0f06107b98
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone3_Tier3
    title: The Everfrost
    revision: sha256:59661517d2ce1ccba126077933e38dee8611dacd7c2a87f165093c77dcff06cc
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ore_Cobalt_Slate
    title: Cobalt Ore - Slate
    revision: sha256:bf069f25287c1ee203894091a9c8b3d755d4aebca84e0a667106cc4fc06c14be
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Wolf_Black
    title: Black Wolf
    revision: sha256:c6a848fa61ba505f80f1e5b593bff4b14f635b5d5a21fb930595b8367afe2a95
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

**Boreal Reach** and **The Everfrost** are the two named inland regions in the Whisperfrost Frontiers release catalog. Cobalt-bearing slate has recorded generation references in both. The Black Wolf has a recorded association with Boreal Reach.

## Boreal Reach and The Everfrost

```hytl:zone-hero
{
  "zone": "Zone3_Tier2"
}
```
```hytl:zone-hero
{
  "zone": "Zone3_Tier3"
}
```

Use these region names when moving between guides, the zone atlas and creature records. The tier labels distinguish regional records; they are not a player-level requirement. The shore and shallow-ocean entries also have separate tier-specific records.

## Cobalt in slate

```hytl:zone-bars
{
  "item": "Ore_Cobalt_Slate",
  "zones": [
    "Zone3_Tier2",
    "Zone3_Tier3"
  ]
}
```

After gathering Cobalt Ore, use a Furnace to process it into ingots. Cobalt ingots appear in the first named backpack upgrade as well as equipment recipes, so decide what you are saving for before spending them. The live :wiki[backpack recipes]{page="backpack-upgrades"} and :wiki[metal sword comparison]{page="metal-swords"} show those competing material requirements.

## Black Wolf

```hytl:creature
{
  "entity": "Wolf_Black"
}
```

The observed drop list includes Medium Hide and raw wildmeat. For leather, follow Medium Hide into its processing recipe. A wolf's region link does not establish where a pack will be standing in a particular generated world.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "thorium-and-cobalt",
          "label": "Thorium and cobalt"
        },
        {
          "kind": "wiki",
          "id": "medium-hide-sources",
          "label": "Medium Hide sources"
        },
        {
          "kind": "wiki",
          "id": "world-generation",
          "label": "World generation"
        }
      ]
    }
  ]
}
```

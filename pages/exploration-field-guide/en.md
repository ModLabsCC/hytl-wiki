---
hytlMarkdown: 1
locale: en
title: Exploration field guide
slug: exploration/field-guide
description: Choose a destination around the material or encounter you need.
  These guides connect the named regions of the overworld to ore deposits,
  crafting stations and creature records, so you can plan a trip and follow the
  materials back to your workshop.
status: complete
sources:
  - url: https://hytl.dev/zones/Zone1_Tier2
    title: Seedling Woods
    revision: sha256:ac9b2659900b4bf3bf2792ea458f179387b720ebb33a638f1c7ff7e6bf68a358
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone2_Tier2
    title: Badlands
    revision: sha256:549505720d74b472ade922c37e5f7f3956b05b0275de0d80ef1d6bc23883904a
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone3_Tier2
    title: Boreal Reach
    revision: sha256:ca6ad29c279f8f7a29081a48a3c476eb2d66f8f18e77083b67e61c0f06107b98
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone4_Tier4
    title: Cinder Wastes
    revision: sha256:1760ee5ab9ea19245656fb37af361f5fba2670fa3bd097f9180dd6ead4e199a8
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Choose a destination around the material or encounter you need. These guides connect the named regions of the overworld to ore deposits, crafting stations and creature records, so you can plan a trip and follow the materials back to your workshop.

## Choose a region

```hytl:hub-tiles
{
  "pages": [
    "emerald-wilds-guide",
    "howling-sands-guide",
    "whisperfrost-frontiers-guide",
    "devastated-lands-guide"
  ],
  "limit": 4
}
```

Seedling Woods and The Fens belong to the Emerald Wilds. Badlands and Desolate Basin belong to the Howling Sands. Boreal Reach and The Everfrost are part of the Whisperfrost Frontiers, while Cinder Wastes and Charred Woodlands belong to the Devastated Lands. Open a region card for its current resource and creature records.

## Bring the trip back to your base

Start with :wiki[workstations]{page="workstations-guide"} if you are missing the station needed by a recipe. The :wiki[copper and iron guide]{page="copper-and-iron"} connects mining to ingots; :wiki[backpack upgrades]{page="backpack-upgrades"} and :wiki[teleporters]{page="teleporters-guide"} help with carrying materials and returning between established locations.

## Read the map before committing to a route

Ore panels identify regions referenced by the game files. They do not provide fixed coordinates in your world. Creature lists identify recorded associations rather than guaranteed encounters. World generation can also change between versions; the :wiki[world-generation overview]{page="world-generation"} explains the official distinction between V1 and V2.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "chapter-one",
          "label": "Chapter I: where to start"
        },
        {
          "kind": "wiki",
          "id": "memories-and-heart",
          "label": "Memories and the Heart of Orbis"
        },
        {
          "kind": "wiki",
          "id": "repair-kits-guide",
          "label": "Repair kits"
        }
      ]
    }
  ]
}
```

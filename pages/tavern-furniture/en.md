---
hytlMarkdown: 1
locale: en
title: Building a tavern interior
slug: crafting/tavern-furniture
description: A small tavern interior can start with a table, chairs, a candle
  and a bed. These selected Tavern items have separate recipes, and they do not
  all use the same workstation or wood form.
status: complete
sources:
  - url: https://hytl.dev/items/Furniture_Tavern_Table
    title: Tavern Table
    revision: sha256:69584168da54a9650347f7d56523a4f12dc825dfa21f82d2e5b100303a34e5ec
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Furniture_Tavern_Chair
    title: Tavern Chair
    revision: sha256:7b6576c32b13ea8240520624707031e8b4cc5ee0a2b5f7dab490e3689ac1fd8c
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Furniture_Tavern_Candle
    title: Tavern Candle
    revision: sha256:f742ea11ea21d3201fc72231ea7a2b00ea51f92831f43e3e22ec9286219f2d83
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Furniture_Tavern_Bed
    title: Tavern Bed
    revision: sha256:7bcf0482b473f580073e7568ef15e68875370a6cb717ca8689b6d6b2c24f42d4
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Builders
    title: Builder's Workbench
    revision: sha256:a788c10759ebf59d6df3eff36697d568693573e655187c2c2994b332e5be38a9
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Furniture
    title: Furniture Workbench
    revision: sha256:7a832cc7a6742180bb86d3f0591e09b4976d36fff10c6e8748c59a59dbfbbb13
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytale.com/news/2026/3/hytale-patch-notes-update-4
    revision: sha256:89a2605a403ed41a16125d609ce3c5fb7e0484a7bf73c2659966242e6dcb524f
    retrievedAt: 2026-10-15T13:46:12.388170+00:00
    license: Factual reference to an official Hytale post; copyright retained by
      Hypixel Studios. Independently written summary, no copied article.
    attribution: Hytale Team / Hypixel Studios
    modifications: Original, selective summary of the dated announcement; future
      plans remain labelled as plans.
---

A small tavern interior can start with a table, chairs, a candle and a bed. These selected Tavern items have separate recipes, and they do not all use the same workstation or wood form.

## Split structural pieces from furnishings

The Table and Chair use the Builder's Workbench with the Darkwood resource group. The Bed and Candle use the Furniture Workbench. Build the appropriate station before assuming every item named “Tavern” belongs in one crafting menu.

```hytl:recipe
{
  "item": "Bench_Builders"
}
```
```hytl:recipe
{
  "item": "Bench_Furniture"
}
```

## Plan the selected pieces

```hytl:furniture-set
{
  "title": "Selected Tavern furnishings",
  "items": [
    "Furniture_Tavern_Table",
    "Furniture_Tavern_Chair",
    "Furniture_Tavern_Candle",
    "Furniture_Tavern_Bed"
  ]
}
```

The table needs four units of Darkwood and the chair needs two. The bed specifically lists Darkwood Planks alongside fibre and red and white cloth. A generic wood-group ingredient and a named plank item are different requirements. The candle uses fibre and Tree Sap, rather than the table's wood requirement.

## More lighting choices

```hytl:recipe-book
{
  "category": "Furniture_Lighting",
  "page": 1,
  "limit": 4
}
```

The [Update 4 building notes](https://hytale.com/news/2026/3/hytale-patch-notes-update-4) describe the expansion of structural block variants and connected pieces. Use the current item recipes when choosing supplies; the existence of a decorative asset alone does not prove a survival crafting route.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "workstations-guide",
          "label": "Workstations"
        },
        {
          "kind": "wiki",
          "id": "copper-and-iron",
          "label": "Copper and iron"
        }
      ]
    }
  ]
}
```

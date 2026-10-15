---
hytlMarkdown: 1
locale: en
title: Wheat and flour
slug: crafting/wheat-and-flour
description: Wheat farming and flour processing use different stations. Craft
  seed bags at the Farmer's Workbench; the observed Flour recipe belongs to the
  Chef's Stove's ingredient category.
status: complete
sources:
  - url: https://hytl.dev/items/Plant_Seeds_Wheat
    title: Wheat Seed Bag
    revision: sha256:6d14685ebc8743bc21bb85a9df393238aabeccbedf7d2008d5ca6c6948da2cad
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Plant_Seeds_Wheat_Eternal
    title: Wheat Seed Bag (Eternal)
    revision: sha256:da092adeec94238bdd6c9ded0d947feffbec8da8c8e66effc72c8ba0b378935f
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Plant_Crop_Wheat_Item
    title: Wheat
    revision: sha256:7e31ed81d3091e3f64c471562bb0fe86e9ac8bb47307d214f69a4488b12ef954
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ingredient_Flour
    title: Flour
    revision: sha256:71434ce95faa314fc079429c13e7c4d934eb0b3f9a08fb197025e43d95cc2693
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Farming
    title: Farmer's Workbench
    revision: sha256:a434658cec340317742aac42768aeb34854d2f3d13b8c3941a17c2e6677c24f9
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Cooking
    title: Chef's Stove
    revision: sha256:907235d2969172e7a2a507cd4304d24173642415db305dea9cb2e16c63068db7
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Wheat farming and flour processing use different stations. Craft seed bags at the Farmer's Workbench; the observed Flour recipe belongs to the Chef's Stove's ingredient category.

## Craft the ordinary seed bag

```hytl:recipe
{
  "item": "Bench_Farming"
}
```
```hytl:recipe
{
  "item": "Plant_Seeds_Wheat"
}
```

The ordinary Wheat Seed Bag recipe uses two Essence of Life. Its placement interaction identifies the Wheat crop block, rather than the harvested Wheat item. Keep that distinction when browsing item records: a seed, crop block and harvested ingredient can have similar names but different functions.

## The Eternal seed bag

```hytl:recipe
{
  "item": "Plant_Seeds_Wheat_Eternal"
}
```

The Eternal recipe uses 20 Essence of Life, ten Wheat and one ordinary Wheat Seed Bag. It also lists a tier-2 farming bench requirement and **RequiredMemoriesLevel: 2**. That is a configured Memories level, not a claim that collecting two creatures unlocks it.

## Process harvested Wheat

```hytl:recipe
{
  "item": "Ingredient_Flour"
}
```

The observed Flour recipe consumes ten Wheat and lists one second of crafting time. Check the intended food recipe before turning all your Wheat into flour; other recipes can ask for Wheat directly.

Growth duration, watering multipliers and harvest yield are not established by these ingredient and recipe records. This guide therefore gives the verified crafting chain without inventing an optimal farm schedule.

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
          "id": "memories-and-heart",
          "label": "Memories and the Heart of Orbis"
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

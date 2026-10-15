---
hytlMarkdown: 1
locale: en
title: "Copper and iron: from ore to ingots"
slug: materials/copper-and-iron
description: "Copper and iron pass through two different forms: an ore you
  gather and an ingot you process. Recipes for tools and benches commonly ask
  for the ingot, so carrying an ore stack does not yet satisfy that ingredient."
status: complete
sources:
  - url: https://hytl.dev/items/Ingredient_Bar_Copper
    title: Copper Ingot
    revision: sha256:744b54ceae1e7e58a2c91a86a8c6f489fe9effe4eac7e35e26db1c258f8d513a
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ingredient_Bar_Iron
    title: Iron Ingot
    revision: sha256:657336f7da240eeaebdddc8958c9075df5333399d30bd23cabe4e23237280bab
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
  - url: https://hytl.dev/items/Bench_Furnace
    title: Furnace
    revision: sha256:250bc9c494ca11d304ad0a10b0883d5d74c5df0f6c130cbd25a6e1732acbb430
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://cdn.hytale.com/5e7ba03050cbcd001176c601_31___cave_explorer.png
    revision: sha256:a262a7ecf2c27b66136e858cf4a4df92d32e938ff5ab4882a3139e9376c01aa6
    license: Hytale editorial media permission (Content Creators FAQ); copyright
      retained by Hypixel Studios. Not CC BY.
    retrievedAt: 2026-10-15T12:48:49.653Z
    attribution: © Hytale / Hypixel Studios. Official development screenshot; no
      endorsement implied.
    title: Cave explorer — official Hytale screenshot
    modifications: "Resized proportionally to 1600 × 900; re-encoded as PNG with
      metadata removed. No crop or compositing. Asset SHA256:
      9cb61abbb6c71e948be5463941f47445cd836da463e2c31f7046dd3a1d8c5f58"
---

Copper and iron pass through two different forms: an ore you gather and an ingot you process. Recipes for tools and benches commonly ask for the ingot, so carrying an ore stack does not yet satisfy that ingredient.

## Find the ore-bearing block

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/9cb61abbb6c71e948be5463941f47445cd836da463e2c31f7046dd3a1d8c5f58.png",
      "alt": "An adventurer exploring a torch-lit cave.",
      "caption": "An adventurer exploring a torch-lit cave. Official development illustration (WIP); not a verified location or present-day recipe.",
      "source": {
        "url": "https://cdn.hytale.com/5e7ba03050cbcd001176c601_31___cave_explorer.png",
        "revision": "sha256:a262a7ecf2c27b66136e858cf4a4df92d32e938ff5ab4882a3139e9376c01aa6",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.653Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "title": "Cave explorer — official Hytale screenshot",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: 9cb61abbb6c71e948be5463941f47445cd836da463e2c31f7046dd3a1d8c5f58"
      }
    }
  ]
}
```

The stone variants below have generation references across several regions. Their maps are a starting point for choosing a destination. Other host-rock variants have their own records, so the name of the embedded rock matters.

```hytl:ore-map
{
  "item": "Ore_Copper_Stone"
}
```
```hytl:ore-map
{
  "item": "Ore_Iron_Stone"
}
```

## Process at a Furnace

```hytl:recipe
{
  "item": "Bench_Furnace"
}
```
```hytl:recipe
{
  "item": "Ingredient_Bar_Copper"
}
```
```hytl:recipe
{
  "item": "Ingredient_Bar_Iron"
}
```

The observed recipes process one matching ore into one ingot. Copper lists 10 seconds and iron lists 14 seconds. These are recipe processing times, not a measurement of an entire gathering trip or a promise about a modded server's throughput.

## Decide where the first ingots go

The Blacksmith's Anvil and Armorer's Workbench each use copper in their station recipe. Iron is also needed by the Repair Kit and the initial backpack unlock. Check :wiki[workstations]{page="workstations-guide"} before spending the last of a material on equipment, and follow :wiki[Crafting an Iron Sword]{page="crafting-an-iron-sword"} once the weapon station and ingredients are ready.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "repair-kits-guide",
          "label": "Repair kits"
        },
        {
          "kind": "wiki",
          "id": "backpack-upgrades",
          "label": "Backpack upgrades"
        },
        {
          "kind": "wiki",
          "id": "emerald-wilds-guide",
          "label": "Emerald Wilds"
        }
      ]
    }
  ]
}
```

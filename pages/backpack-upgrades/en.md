---
hytlMarkdown: 1
locale: en
title: Backpack upgrades
slug: equipment/backpack-upgrades
description: Backpack upgrades increase a separate carrying capacity in steps.
  Crafting the upgrade item is followed by using that consumable; its configured
  interaction checks the previous capacity and sets the next one.
status: complete
sources:
  - url: https://hytl.dev/items/Upgrade_Backpack_1
    title: Unlock Backpack
    revision: sha256:b2d4cfaecb7a48928c39ffc0a1c67a96adffe0450634e590d08ad621b4a1e7fe
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Upgrade_Backpack_2
    title: Backpack Upgrade I
    revision: sha256:365efce461509f2ce9a2f92f8b6e10cdf8d0c9d11cbd3810d2e43b1865c87ae3
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Upgrade_Backpack_3
    title: Backpack Upgrade II
    revision: sha256:1d56b92ecb420f0eba1407983078464077df5eb387cc90d4a240889cbbfa6b82
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Upgrade_Backpack_4
    title: Backpack Upgrade III
    revision: sha256:5f6cbef5f8b543f856a7ae1a3591b06c42fee7a0cd83dd3cde2f24d451a1fee0
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Backpack upgrades increase a separate carrying capacity in steps. Crafting the upgrade item is followed by using that consumable; its configured interaction checks the previous capacity and sets the next one.

## Unlock the first capacity

```hytl:recipe
{
  "item": "Upgrade_Backpack_1"
}
```

The observed unlock requires eight Iron Ingots and eight Medium Leather at a tier-1 Workbench. Both primary and secondary interactions are configured to increase backpack capacity from 0 to 9. Gather the ingots and process the matching hides before crafting it.

## Upgrade an existing backpack

```hytl:recipe
{
  "item": "Upgrade_Backpack_2"
}
```

Backpack Upgrade I changes capacity from 9 to 18. Its observed recipe uses Cindercloth Scraps, Cobalt Ingots and Heavy Leather, and requires a tier-2 Workbench. Each upgrade level is described as usable once.

## Later upgrade records

| Item | Configured capacity change | Observed recipe |
| --- | --- | --- |
| Backpack Upgrade II | 18 → 27 | Goblin Lab workbench, with power and recipe-C augment tags |
| Backpack Upgrade III | 27 → 36 | No recipe in the observed record |

```hytl:recipe
{
  "item": "Upgrade_Backpack_3"
}
```

For Upgrade II, the recorded materials are Scraps, Spider Silk and Voidtaken Grizzly Hide. The missing recipe on Upgrade III does not prove it is unobtainable; it means this guide cannot provide a verified crafting or unlock route for it.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "copper-and-iron",
          "label": "Copper and iron"
        },
        {
          "kind": "wiki",
          "id": "leather-from-hides",
          "label": "Leather from hides"
        },
        {
          "kind": "wiki",
          "id": "chapter-one",
          "label": "Chapter I: where to start"
        }
      ]
    }
  ]
}
```

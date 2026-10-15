---
hytlMarkdown: 1
locale: en
title: Teleporters
slug: exploration/teleporters
description: Teleporters connect placed pads into a warp link. The current item
  description instructs you to place two, and the observed crafting recipe
  produces two teleporters per craft.
status: complete
sources:
  - url: https://hytl.dev/items/Teleporter
    title: Teleporter
    revision: sha256:ad06452981b1e5180326589adb0d610ea1e8f35ae62425bfa9b2310c1f6012df
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Arcane
    title: Arcanist's Workbench
    revision: sha256:30ef5b2e0f7e757e0f7dfea8947a912f1882af48d6dc3a85b9491aca128cebeb
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Wood_Azure_Trunk
    title: Azure Log
    revision: sha256:747dc33aa6e922933c9463a14cbf63d2dc3539c38b31e09e30d7b8cacedca363
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Plant_Crop_Mana3
    title: Azure Kelp
    revision: sha256:a95e7d8ce77a5a8c1c7ecf1c6f380d9462d2793bce5009c157277a4de29cc810
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Teleporters connect placed pads into a warp link. The current item description instructs you to place two, and the observed crafting recipe produces two teleporters per craft.

## Build the Arcanist's Workbench

```hytl:recipe
{
  "item": "Bench_Arcane"
}
```

The station recipe requires a tier-2 Workbench and uses Thorium Ingots, Linen Scraps and Essence of the Void. Plan for the station cost before gathering only the teleporter ingredients.

## Craft the pair

```hytl:infobox
{
  "type": "item",
  "id": "Teleporter"
}
```
```hytl:recipe
{
  "item": "Teleporter"
}
```

The observed recipe asks for eight Azure Logs, two Azure Kelp and ten units of the Rock resource group. Follow the ingredient links for their source records. The output quantity is two, so one craft provides the pair described by the item.

## Place and configure the link

Place both teleporters, then interact with a pad to open its warp interface. The game-file configuration connects the pad's Use interaction to that interface, while the active state uses a collision-entry teleporter interaction.

Name and select the destination in the game interface rather than relying on a screenshot of an older UI. This guide does not assert a cross-world travel rule, a distance limit or a numerical pad limit, because those are not established by the cited item record.

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
          "id": "workstations-guide",
          "label": "Workstations"
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

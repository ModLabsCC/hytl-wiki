---
hytlMarkdown: 1
locale: en
title: Repair kits
slug: equipment/repair-kits
description: The standard Repair Kit repairs tools, weapons and armour. Its item
  description also warns that repaired items lose up to 10% of their maximum
  durability, so repair is a trade-off rather than a permanent reset to a new
  item.
status: complete
sources:
  - url: https://hytl.dev/items/Tool_Repair_Kit_Iron
    title: Repair Kit
    revision: sha256:5fa6f7b8ea7b733a7157e97097eec46efe8829543f915fdc1c1ff4f358a89ee9
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Tool_Repair_Kit_Crude
    title: Crude Repair Kit
    revision: sha256:d10cc6d8e48ec08f6163add29550abf56e94e12198251fb9357d2ec3a8b4cec7
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

The standard Repair Kit repairs tools, weapons and armour. Its item description also warns that repaired items lose up to 10% of their maximum durability, so repair is a trade-off rather than a permanent reset to a new item.

## Craft a standard kit

```hytl:infobox
{
  "type": "item",
  "id": "Tool_Repair_Kit_Iron"
}
```
```hytl:recipe
{
  "item": "Tool_Repair_Kit_Iron"
}
```

The observed Workbench recipe consumes two Linen Scraps, one Iron Ingot and one Light Leather to produce one kit. If you have ore and hide instead, process them first: the recipe asks for the finished ingot and leather.

## Open the repair interface

Both primary and secondary use are configured to open the item-repair interface. Select the item you want to repair there. The record sets a repair penalty of 0.1, consistent with the description's maximum-durability warning.

Before spending rare materials on repeated repairs, compare the cost of a replacement with the kit ingredients. That is a planning choice; the live recipe below does not estimate how many uses remain on your personal item.

## Distinguish kit variants

The Crude Repair Kit is a separate item record. Do not assume its properties from the standard kit's recipe or name. Likewise, Chapter-I-specific repair items need their own records rather than inheriting this kit's penalty.

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
          "label": "Iron for the kit"
        },
        {
          "kind": "wiki",
          "id": "leather-from-hides",
          "label": "Light Leather"
        },
        {
          "kind": "wiki",
          "id": "metal-swords",
          "label": "Metal sword recipes"
        }
      ]
    }
  ]
}
```

---
hytlMarkdown: 1
locale: en
title: Adamantite equipment
slug: equipment/adamantite
description: Adamantite Ore is processed into Adamantite Ingots before it is
  used by the sword recipe. Keep the ore-bearing block, its dropped resource and
  the finished ingot separate when following crafting requirements.
status: complete
sources:
  - url: https://hytl.dev/items/Ore_Adamantite_Magma
    title: Adamantite Ore - Magma
    revision: sha256:a59bc1a0b34093b5bf95e9728f03950ccffda8a43f90b093ade212e1b778d477
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ingredient_Bar_Adamantite
    title: Adamantite Ingot
    revision: sha256:885a8d5e3deba57aeed5bd873934cf3abdb64ce76ce28a288cd1311dc0297e62
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Weapon_Sword_Adamantite
    title: Adamantite Sword
    revision: sha256:3be28a208d8500bb6935fe73bbbcf11e4d0568b29679f2b9a8c82e61852a3c46
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytale.com/news/2026/1/hytale-patch-notes-update-2
    revision: sha256:459c0f7394acdb882f123c003e201c5787a85870058bb4f2dad50f577c8ce800
    retrievedAt: 2026-10-15T13:46:12.188920+00:00
    license: Factual reference to an official Hytale post; copyright retained by
      Hypixel Studios. Independently written summary, no copied article.
    attribution: Hytale Team / Hypixel Studios
    modifications: Original, selective summary of the dated announcement; future
      plans remain labelled as plans.
---

Adamantite Ore is processed into Adamantite Ingots before it is used by the sword recipe. Keep the ore-bearing block, its dropped resource and the finished ingot separate when following crafting requirements.

## Recognise the material chain

```hytl:infobox
{
  "type": "item",
  "id": "Ore_Adamantite_Magma"
}
```

The magma-hosted block's breaking configuration lists Adamantite Ore and Cooled Magma Rock as outputs. Its gathering configuration uses the Adamantite ore gather type and quality 4. This identifies the block and its configured drops; it does not establish a mining coordinate.

## Process the ore

```hytl:recipe
{
  "item": "Ingredient_Bar_Adamantite"
}
```

One ore produces one ingot in the observed Furnace recipe, with a 20-second processing time. Save the ingots for the item you intend to make, then gather the remaining ingredients before returning to the weapon bench.

## Craft the sword

```hytl:recipe
{
  "item": "Weapon_Sword_Adamantite"
}
```

The observed sword recipe requires 11 Adamantite Ingots, four Heavy Leather and three Cindercloth Scraps, at a tier-3 weapon bench. The :wiki[leather guide]{page="leather-from-hides"} explains the hide-to-leather step.

## Mining changes in the official notes

The [24 January Update 2 notes](https://hytale.com/news/2026/1/hytale-patch-notes-update-2) introduced a Thorium-or-Cobalt-pickaxe requirement for Adamantite. This is dated patch history; consult the current tool and block records when checking a later build or a modified server.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "metal-swords",
          "label": "Metal swords"
        },
        {
          "kind": "wiki",
          "id": "devastated-lands-guide",
          "label": "Devastated Lands"
        },
        {
          "kind": "wiki",
          "id": "thorium-and-cobalt",
          "label": "Thorium and cobalt"
        }
      ]
    }
  ]
}
```

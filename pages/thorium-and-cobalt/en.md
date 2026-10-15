---
hytlMarkdown: 1
locale: en
title: Thorium and cobalt
slug: materials/thorium-and-cobalt
description: Thorium and cobalt are separate material choices with different
  gathering routes. Thorium-bearing sandstone is recorded in Badlands and
  Desolate Basin; cobalt-bearing slate is recorded in Boreal Reach and The
  Everfrost, along with several Whisperfrost shore and shallow-ocean records.
status: complete
sources:
  - url: https://hytl.dev/items/Ore_Thorium_Sandstone
    title: Thorium Ore - Sandstone
    revision: sha256:28291f7c0cff90f5880ee61d1129931108c7162671feab4af353b0351bf3fbd0
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
  - url: https://hytl.dev/items/Ingredient_Bar_Thorium
    title: Thorium Ingot
    revision: sha256:1d78f3c14c340a437a72040808f0b70a2b9144a159eb5635bcb25e62b4eca9c0
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ingredient_Bar_Cobalt
    title: Cobalt Ingot
    revision: sha256:b152d37b32d0eaf40d21534e60b9c05deb5b511c581e1d1131965e48bb52b62a
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Weapon_Sword_Thorium
    title: Thorium Sword
    revision: sha256:f22d7450970d4cc31e66c69f8f840ab99c72602b036d0a39bde3c03680f6fc1e
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Weapon_Sword_Cobalt
    title: Cobalt Sword
    revision: sha256:0d70353337c2aa6f6914f29f903f002c973f39e849ea2732c931ac306ef3da8e
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Thorium and cobalt are separate material choices with different gathering routes. Thorium-bearing sandstone is recorded in Badlands and Desolate Basin; cobalt-bearing slate is recorded in Boreal Reach and The Everfrost, along with several Whisperfrost shore and shallow-ocean records.

## Choose a gathering route

```hytl:ore-map
{
  "item": "Ore_Thorium_Sandstone"
}
```
```hytl:ore-map
{
  "item": "Ore_Cobalt_Slate"
}
```

Use the :wiki[Howling Sands guide]{page="howling-sands-guide"} for the thorium route or :wiki[Whisperfrost Frontiers guide]{page="whisperfrost-frontiers-guide"} for cobalt. These maps show recorded generation associations, not a coordinate list or ore-per-chunk estimate.

## Smelt the ore

```hytl:recipe
{
  "item": "Ingredient_Bar_Thorium"
}
```
```hytl:recipe
{
  "item": "Ingredient_Bar_Cobalt"
}
```

Both observed Furnace recipes convert one ore to one ingot and list an 18-second processing time. The later equipment recipe determines how many ingots you need.

## Check the other materials too

The Thorium Sword recipe uses Medium Leather and Linen Scraps alongside thorium. The Cobalt Sword recipe uses Heavy Leather and Shadoweave Scraps alongside cobalt. Both list a tier-2 weapon bench requirement. Changing metal therefore changes more than the ore you gather.

```hytl:recipe
{
  "item": "Weapon_Sword_Thorium"
}
```
```hytl:recipe
{
  "item": "Weapon_Sword_Cobalt"
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
          "id": "metal-swords",
          "label": "Metal swords"
        },
        {
          "kind": "wiki",
          "id": "leather-from-hides",
          "label": "Leather from hides"
        },
        {
          "kind": "wiki",
          "id": "backpack-upgrades",
          "label": "Backpack upgrades"
        }
      ]
    }
  ]
}
```

---
hytlMarkdown: 1
locale: en
title: Comparing metal sword recipes
slug: equipment/metal-swords
description: "Copper, iron, thorium, cobalt and adamantite swords use different
  material combinations. Compare the full recipe before choosing a metal:
  leather grade, fabric scraps and weapon-bench tier can change alongside the
  ingots."
status: complete
sources:
  - url: https://hytl.dev/items/Weapon_Sword_Copper
    title: Copper Sword
    revision: sha256:44496405bcfbe9649364d9e9473d9c4e6d4783a70744c8881ec1ddee9fe6bddb
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Weapon_Sword_Iron
    title: Iron Sword
    revision: sha256:57ca44b09c00d7b24ead42e75065c0072362b3cb607f1863df064c01b5076f5c
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
  - url: https://hytl.dev/items/Weapon_Sword_Adamantite
    title: Adamantite Sword
    revision: sha256:3be28a208d8500bb6935fe73bbbcf11e4d0568b29679f2b9a8c82e61852a3c46
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

Copper, iron, thorium, cobalt and adamantite swords use different material combinations. Compare the full recipe before choosing a metal: leather grade, fabric scraps and weapon-bench tier can change alongside the ingots.

## Compare the catalog fields

```hytl:weapon-compare
{
  "items": [
    "Weapon_Sword_Copper",
    "Weapon_Sword_Iron",
    "Weapon_Sword_Thorium",
    "Weapon_Sword_Cobalt",
    "Weapon_Sword_Adamantite"
  ]
}
```

Quality and item level describe the catalog records. They are not measured damage-per-second values, and item level is not asserted here as a player-level requirement. A combat comparison would additionally need dependable attack damage, timing and conditions.

## Copper and iron

The Copper Sword combines four Copper Ingots, four Wood Trunk resource units and three Plant Fibre. The Iron Sword changes the supporting ingredients to Light Leather and Linen Scraps.

```hytl:recipe
{
  "item": "Weapon_Sword_Copper"
}
```
```hytl:recipe
{
  "item": "Weapon_Sword_Iron"
}
```

## Later material choices

Thorium and cobalt recipes both list a tier-2 weapon bench, while the Adamantite Sword lists tier 3. Their leather and fabric ingredients differ: Medium Leather and Linen for thorium, Heavy Leather and Shadoweave for cobalt, Heavy Leather and Cindercloth for adamantite.

Use :wiki[Thorium and cobalt]{page="thorium-and-cobalt"} to plan the first two gathering routes, or :wiki[Adamantite equipment]{page="adamantite-equipment"} for its ingot and sword recipes. A rarity colour alone does not tell you which route best fits the materials you already have.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "crafting-an-iron-sword",
          "label": "Crafting an Iron Sword"
        },
        {
          "kind": "wiki",
          "id": "thorium-and-cobalt",
          "label": "Thorium and cobalt"
        },
        {
          "kind": "wiki",
          "id": "adamantite-equipment",
          "label": "Adamantite equipment"
        }
      ]
    }
  ]
}
```

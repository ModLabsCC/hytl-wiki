---
hytlMarkdown: 1
locale: en
title: Workstations and processing
slug: crafting/workstations
description: "Crafting is divided between stations. Build the station a recipe
  asks for, then check its tier requirement separately: owning a Workbench does
  not replace the Furnace, Blacksmith's Anvil or Tanning Rack."
status: complete
sources:
  - url: https://hytl.dev/items/Bench_WorkBench
    title: Workbench
    revision: sha256:58ba82a1b030d45bcec5632fa04f2351c7e6fc1d827b1653965ed1d6bdeab5a6
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
  - url: https://hytl.dev/items/Bench_Weapon
    title: Blacksmith's Anvil
    revision: sha256:286574e35dbe46f4e6dd26fe25ead5c296156dda981f1740e9f5e5bc768e20d3
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Armour
    title: Armorer's Workbench
    revision: sha256:6f15c5707e34b888e22be3809caa0566247d1647fc6561f091ac131239c59bf8
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Bench_Tannery
    title: Tanning Rack
    revision: sha256:e9090809cb1ce069bee01866a73729dacef5af58a76b0fd61ac75abc374d5daa
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
  - url: https://hytl.dev/items/Bench_Farming
    title: Farmer's Workbench
    revision: sha256:a434658cec340317742aac42768aeb34854d2f3d13b8c3941a17c2e6677c24f9
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://cdn.hytale.com/5e7ba29b50cbcd001176c699_83___crafted_sword.jpg
    revision: sha256:66fb21aeef7af480622f5ae897ec0b6eaef4dc2bf17446ff4b55d7712cf31178
    license: Hytale editorial media permission (Content Creators FAQ); copyright
      retained by Hypixel Studios. Not CC BY.
    retrievedAt: 2026-10-15T12:48:49.684Z
    attribution: © Hytale / Hypixel Studios. Official development screenshot; no
      endorsement implied.
    title: Crafted sword — official Hytale screenshot
    modifications: "Resized proportionally to 1600 × 900; re-encoded as PNG with
      metadata removed. No crop or compositing. Asset SHA256:
      1b71029ca48e06e4ea226ad0e597954dcca93a612a30a4b8a38bfaeb0776c626"
---

Crafting is divided between stations. Build the station a recipe asks for, then check its tier requirement separately: owning a Workbench does not replace the Furnace, Blacksmith's Anvil or Tanning Rack.

## Start with the Workbench

```hytl:recipe
{
  "item": "Bench_WorkBench"
}
```

The observed fieldcraft recipe uses four units of the Wood Trunk resource group and three of the Rock resource group. A resource group can accept matching materials; it is not a requirement for one specific tree or stone item.

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/1b71029ca48e06e4ea226ad0e597954dcca93a612a30a4b8a38bfaeb0776c626.png",
      "alt": "A sword and a workbench inside a wooden workshop.",
      "caption": "A sword and a workbench inside a wooden workshop. Official development illustration (WIP); not a verified location or present-day recipe.",
      "source": {
        "url": "https://cdn.hytale.com/5e7ba29b50cbcd001176c699_83___crafted_sword.jpg",
        "revision": "sha256:66fb21aeef7af480622f5ae897ec0b6eaef4dc2bf17446ff4b55d7712cf31178",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.684Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "title": "Crafted sword — official Hytale screenshot",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: 1b71029ca48e06e4ea226ad0e597954dcca93a612a30a4b8a38bfaeb0776c626"
      }
    }
  ]
}
```

## Pick the next station for the job

| Job | Station |
| --- | --- |
| Process copper, iron and other ores | Furnace |
| Craft the metal swords in these guides | Blacksmith's Anvil |
| Make armour | Armorer's Workbench |
| Process hides into leather | Tanning Rack |
| Craft the selected beds and lights | Furniture Workbench |
| Craft the wheat seed bags | Farmer's Workbench |

These station uses are established by the linked recipes; the table is not a complete catalog of every recipe in the game.

```hytl:recipe
{
  "item": "Bench_Weapon"
}
```
```hytl:recipe
{
  "item": "Bench_Tannery"
}
```

## Browse Furnace processing recipes

```hytl:recipe-book
{
  "bench": "Bench_Furnace",
  "page": 1,
  "limit": 4
}
```

The recipe book follows the Furnace facet in the current release index. Use the result links to inspect ingredients and output amounts, rather than assuming every recipe has the same conversion or processing time.

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
          "id": "tavern-furniture",
          "label": "Tavern furniture"
        },
        {
          "kind": "wiki",
          "id": "wheat-and-flour",
          "label": "Wheat and flour"
        }
      ]
    }
  ]
}
```

---
hytlMarkdown: 1
locale: en
title: Memories and the Heart of Orbis
slug: exploration/memories
description: The Heart of Orbis is the game's Memories bench. Its observed Use
  interaction sets a Memories capacity of 48 and opens the Memories interface or
  the initial unlock screen, depending on the interaction's result.
status: complete
sources:
  - url: https://hytl.dev/items/Bench_Memories
    title: The Heart of Orbis
    revision: sha256:69a8453480d0bb91d0f92448a19c1ea212fe845847b6a6d3277987bfda2309a4
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Bear_Grizzly
    title: Grizzly Bear
    revision: sha256:54a45f551304802c977a9eb1f38f63b102a5533119b6fb44cda5f305c83a13b1
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
  - url: https://hytale.com/news/2026/1/hytale-patch-notes-update-2
    revision: sha256:459c0f7394acdb882f123c003e201c5787a85870058bb4f2dad50f577c8ce800
    retrievedAt: 2026-10-15T13:46:12.188920+00:00
    license: Factual reference to an official Hytale post; copyright retained by
      Hypixel Studios. Independently written summary, no copied article.
    attribution: Hytale Team / Hypixel Studios
    modifications: Original, selective summary of the dated announcement; future
      plans remain labelled as plans.
  - url: https://hytale.com/news/2026/8/update-6-patch-notes
    revision: sha256:93b5ee161fe32e46a547ef44285ec1de1a9d7571423e9e07a163654dd94326f5
    retrievedAt: 2026-10-15T13:46:12.481751+00:00
    license: Factual reference to an official Hytale post; copyright retained by
      Hypixel Studios. Independently written summary, no copied article.
    attribution: Hytale Team / Hypixel Studios
    modifications: Original, selective summary of the dated announcement; future
      plans remain labelled as plans.
---

The Heart of Orbis is the game's Memories bench. Its observed Use interaction sets a Memories capacity of 48 and opens the Memories interface or the initial unlock screen, depending on the interaction's result.

```hytl:infobox
{
  "type": "item",
  "id": "Bench_Memories"
}
```

## Creature memories and recipe requirements

The Grizzly Bear's role explicitly enables memory collection and places it in the Predator category. This verifies a memory-bearing creature example without assuming that every technical entity or invisible marker in the catalog is collectible.

The Eternal Wheat Seed Bag recipe contains **RequiredMemoriesLevel: 2**. A Memories level is a progression field; it should not be rewritten as “two memories”. This source does not establish a level-to-count reward table.

## Keep a personal note

```hytl:memories
{
  "id": "Bear_Grizzly",
  "tracker": true,
  "source": {
    "url": "https://hytl.dev/entities/Bear_Grizzly",
    "title": "Grizzly Bear",
    "revision": "sha256:54a45f551304802c977a9eb1f38f63b102a5533119b6fb44cda5f305c83a13b1",
    "retrievedAt": "2026-10-15T13:44:32.669108+00:00",
    "license": "Factual game-data reference; Hytale assets retain their original rights. No source prose or media reproduced.",
    "attribution": "Hytale game-file records, observed in the HYTL.DEV release index",
    "modifications": "Original editorial explanation. Current live components may show later indexed values."
  }
}
```

The optional checkbox is a personal wiki checklist stored in this browser. It does not read your save or mark a memory as restored in Hytale. Use it only to keep track of what you have checked yourself.

## Official changes

The [Update 2 notes](https://hytale.com/news/2026/1/hytale-patch-notes-update-2) describe alphabetically sorted Memories categories at the Heart of Orbis. [Update 6](https://hytale.com/news/2026/8/update-6-patch-notes) added support for optional translated descriptions and fixed Zombie variants failing to generate memories.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "grizzly-bear-guide",
          "label": "Grizzly Bear"
        },
        {
          "kind": "wiki",
          "id": "wheat-and-flour",
          "label": "Wheat and flour"
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

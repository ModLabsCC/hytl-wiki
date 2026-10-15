---
hytlMarkdown: 1
locale: en
title: Finding silver
slug: materials/finding-silver
description: Use indexed ore and region records to plan a silver search while
  keeping generation evidence separate from probability.
status: complete
sources:
  - url: https://hytl.dev/items/Ore_Silver_Stone
    revision: sha256:484fd7140d34dd362f4f57c6ebda8ca73de0bf7cb82eee8ab481aef7014ba867
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Silver Ore - Stone
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/zones/Zone1_Tier2
    revision: sha256:c1ba6b5f0720fea77fec5dac8ac1b5930875555d8d4f7dcecbff2f6655e1ebb5
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Seedling Woods
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/zones/Zone1_Tier3
    revision: sha256:7734b3f966e93f8594c418217045687cc9ec1a1868415bdfedb0c12b6aa0f054
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: The Fens
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
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

## Start with the ore record

The release index distinguishes a silver-bearing block such as :item[Silver Ore - Stone]{id="Ore_Silver_Stone"} from processed materials and equipment whose names also contain silver. Open the ore record when the question is where to gather the resource, then follow the finished item's recipe for later processing steps.

::infobox{type="item" id="Ore_Silver_Stone"}

## Read the region evidence

The ore-map component draws on world-generation references in the indexed game files. It is useful for finding which regions are associated with the ore. Counts of file references are not percentages of blocks in the world, so a larger count should not be read as a measured chance per chunk.

::ore-map{item="Ore_Silver_Stone"}

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/9cb61abbb6c71e948be5463941f47445cd836da463e2c31f7046dd3a1d8c5f58.png",
      "alt": "An adventurer carrying a torch inside a rocky cave with cobwebs.",
      "caption": "Cave exploration in an official development screenshot. This illustrates exploration; the image does not identify a Silver Ore deposit. Work in progress; the final game may differ.",
      "source": {
        "url": "https://cdn.hytale.com/5e7ba03050cbcd001176c601_31___cave_explorer.png",
        "title": "Cave explorer — official Hytale screenshot",
        "revision": "sha256:a262a7ecf2c27b66136e858cf4a4df92d32e938ff5ab4882a3139e9376c01aa6",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.653Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: 9cb61abbb6c71e948be5463941f47445cd836da463e2c31f7046dd3a1d8c5f58"
      }
    }
  ]
}
```

## Move between the region and the resource

Region pages collect the resources and creatures associated with that region. The ore page collects the locations associated with the resource. Following both directions helps you decide what to investigate without assuming that every cave or structure contains the same deposits.

Only the observed relationship is established here. This guide does not infer mining height, spawn chance or the required tool from a material's name. Check the live record for fields the current extraction actually provides.

::data-values{type="item" id="Ore_Silver_Stone"}

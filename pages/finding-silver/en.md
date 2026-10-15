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
    title: Silver Ore - Stone
    revision: sha256:484fd7140d34dd362f4f57c6ebda8ca73de0bf7cb82eee8ab481aef7014ba867
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/zones/Zone1_Tier2
    title: Seedling Woods
    revision: sha256:c1ba6b5f0720fea77fec5dac8ac1b5930875555d8d4f7dcecbff2f6655e1ebb5
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/zones/Zone1_Tier3
    title: The Fens
    revision: sha256:7734b3f966e93f8594c418217045687cc9ec1a1868415bdfedb0c12b6aa0f054
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
---

## Start with the ore record

The release index distinguishes a silver-bearing block such as :item[Silver Ore - Stone]{id="Ore_Silver_Stone"} from processed materials and equipment whose names also contain silver. Open the ore record when the question is where to gather the resource, then follow the finished item's recipe for later processing steps.

::infobox{type="item" id="Ore_Silver_Stone"}

## Read the region evidence

The ore-map component draws on world-generation references in the indexed game files. It is useful for finding which regions are associated with the ore. Counts of file references are not percentages of blocks in the world, so a larger count should not be read as a measured chance per chunk.

::ore-map{item="Ore_Silver_Stone"}

## Move between the region and the resource

Region pages collect the resources and creatures associated with that region. The ore page collects the locations associated with the resource. Following both directions helps you decide what to investigate without assuming that every cave or structure contains the same deposits.

Only the observed relationship is established here. This guide does not infer mining height, spawn chance or the required tool from a material's name. Check the live record for fields the current extraction actually provides.

::data-values{type="item" id="Ore_Silver_Stone"}

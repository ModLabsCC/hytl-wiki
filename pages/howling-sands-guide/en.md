---
hytlMarkdown: 1
locale: en
title: Howling Sands
slug: exploration/howling-sands
description: The Howling Sands includes Badlands and Desolate Basin.
  Thorium-bearing sandstone is associated with both regions in the release data.
  Hyenas also have recorded spawn associations with both, making them a useful
  creature record to check while planning a material-gathering trip.
status: complete
sources:
  - url: https://hytl.dev/zones/Zone2_Tier2
    title: Badlands
    revision: sha256:549505720d74b472ade922c37e5f7f3956b05b0275de0d80ef1d6bc23883904a
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/zones/Zone2_Tier3
    title: Desolate Basin
    revision: sha256:ebc395104287da7d8a7988ab79265441090d138b0c8f325ad93a8521d0a957a7
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ore_Thorium_Sandstone
    title: Thorium Ore - Sandstone
    revision: sha256:28291f7c0cff90f5880ee61d1129931108c7162671feab4af353b0351bf3fbd0
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Hyena
    title: Hyena
    revision: sha256:9037121b1dea3b38e63e91baf8ded09bfb107f6c833497c0252e388ded3f94cd
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://cdn.hytale.com/5e7b9ecb50cbcd001176c5c1_11___z2_camels.png
    revision: sha256:634373462011c362c23f04561aefc3591346df294f8b64a1a8880f16c1ae9735
    license: Hytale editorial media permission (Content Creators FAQ); copyright
      retained by Hypixel Studios. Not CC BY.
    retrievedAt: 2026-10-15T12:48:49.781Z
    attribution: © Hytale / Hypixel Studios. Official development screenshot; no
      endorsement implied.
    title: Camels — official Hytale screenshot
    modifications: "Resized proportionally to 1600 × 900; re-encoded as PNG with
      metadata removed. No crop or compositing. Asset SHA256:
      e750c7bdc4c84ae4fc045b979203ea416a2e51f51eee2399dc6170d12e9beb53"
---

The Howling Sands includes **Badlands** and **Desolate Basin**. Thorium-bearing sandstone is associated with both regions in the release data. Hyenas also have recorded spawn associations with both, making them a useful creature record to check while planning a material-gathering trip.

## Pick the named region

```hytl:zone-hero
{
  "zone": "Zone2_Tier2"
}
```
```hytl:zone-hero
{
  "zone": "Zone2_Tier3"
}
```

The region cards open the individual resource lists. Shore and shallow-ocean records are separate entries; a resource linked to Badlands should not automatically be assumed to occur on every nearby coastline.

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/e750c7bdc4c84ae4fc045b979203ea416a2e51f51eee2399dc6170d12e9beb53.png",
      "alt": "Camels crossing a dry landscape at sunset.",
      "caption": "Camels crossing a dry landscape at sunset. Official development illustration (WIP); not a verified location or present-day recipe.",
      "source": {
        "url": "https://cdn.hytale.com/5e7b9ecb50cbcd001176c5c1_11___z2_camels.png",
        "revision": "sha256:634373462011c362c23f04561aefc3591346df294f8b64a1a8880f16c1ae9735",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.781Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "title": "Camels — official Hytale screenshot",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: e750c7bdc4c84ae4fc045b979203ea416a2e51f51eee2399dc6170d12e9beb53"
      }
    }
  ]
}
```

## Look for thorium-bearing sandstone

```hytl:ore-map
{
  "item": "Ore_Thorium_Sandstone",
  "zones": [
    "Zone2_Tier2",
    "Zone2_Tier3"
  ]
}
```

Thorium Ore and Thorium Ingot are different steps in the material chain. Bring the ore to the Furnace, then check the recipe of the intended tool, weapon or station before processing your whole supply. The :wiki[thorium and cobalt guide]{page="thorium-and-cobalt"} compares their gathering and processing paths.

## Check the encounter before hunting

```hytl:creature
{
  "entity": "Hyena"
}
```

Hyena drops include Medium Hide in the observed release record. Use the hide in the corresponding leather recipe rather than looking for finished leather as the creature drop. If you need chitin instead, consult the separately verified :wiki[Sturdy Chitin sources]{page="sturdy-chitin-guide"}; an insect-like appearance alone does not prove a drop.

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
          "id": "medium-hide-sources",
          "label": "Medium Hide sources"
        },
        {
          "kind": "wiki",
          "id": "sturdy-chitin-guide",
          "label": "Sturdy Chitin"
        }
      ]
    }
  ]
}
```

---
hytlMarkdown: 1
locale: en
title: Medium Hide sources
slug: materials/medium-hide-sources
description: Medium Hide is a creature drop used before the leather-processing
  step. Bison, Boar, Cow, Horse and Warthog all list it in the observed release
  drop data; Black Wolf and Hyena provide further verified examples.
status: complete
sources:
  - url: https://hytl.dev/items/Ingredient_Hide_Medium
    title: Medium Hide
    revision: sha256:dab6ecb38283090fbd57ab3465d702f4832dd3b3c1992aa47c5e3cf14d246980
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Bison
    title: Bison
    revision: sha256:d3d96c45ebfdd4cf24e7d4d30630a252468ed3403416a2cd54f5d738b7c07cf5
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Boar
    title: Boar
    revision: sha256:751e5a94986792bc6eed445a00679640faedc40c80e0758cf58fc095f38ff6e6
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Cow
    title: Cow
    revision: sha256:2c900df82262aaaa82589a9dfb97a7e07c00442999b6c90ca657d2a8e421f04a
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Horse
    title: Horse
    revision: sha256:36427dcf3505ad003ea184ab90779251ef3f37b8e68a2c8af3a3abce16bb8b9e
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Warthog
    title: Warthog
    revision: sha256:4b739a725aab2bf7e9541ed08324a3d8c7e34d10b47a5d0fba5ef378222c0a50
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/entities/Wolf_Black
    title: Black Wolf
    revision: sha256:c6a848fa61ba505f80f1e5b593bff4b14f635b5d5a21fb930595b8367afe2a95
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
  - url: https://hytale.com/news/2026/1/hytale-patch-notes-update-2
    revision: sha256:459c0f7394acdb882f123c003e201c5787a85870058bb4f2dad50f577c8ce800
    retrievedAt: 2026-10-15T13:46:12.188920+00:00
    license: Factual reference to an official Hytale post; copyright retained by
      Hypixel Studios. Independently written summary, no copied article.
    attribution: Hytale Team / Hypixel Studios
    modifications: Original, selective summary of the dated announcement; future
      plans remain labelled as plans.
---

Medium Hide is a creature drop used before the leather-processing step. Bison, Boar, Cow, Horse and Warthog all list it in the observed release drop data; Black Wolf and Hyena provide further verified examples.

## Identify the animal

```hytl:creature-grid
{
  "entities": [
    "Bison",
    "Boar",
    "Cow",
    "Horse",
    "Warthog",
    "Wolf_Black",
    "Hyena"
  ],
  "limit": 8
}
```

This selection is a checked set of examples, not a complete list of every source. Follow an animal card for its own record and use the material's source panel to compare the broader indexed list.

```hytl:loot
{
  "type": "item",
  "id": "Ingredient_Hide_Medium"
}
```

## Check the drop before processing

```hytl:drops
{
  "entity": "Bison"
}
```
```hytl:drops
{
  "entity": "Boar"
}
```

The source lists establish the material relationship. They do not supply a universal amount per kill or a guaranteed probability. Bring back the matching hide, then use the Medium Leather recipe in :wiki[Leather from hides]{page="leather-from-hides"}.

## Why older guides may disagree

The [24 January Update 2 notes](https://hytale.com/news/2026/1/hytale-patch-notes-update-2) explicitly changed Bison, Boar, Cow, Horse and Warthog from Light Hide to Medium Hide. That historical change agrees with the observed release records here. An older animal list can therefore be internally consistent for its date while giving the wrong material for a later build.

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Related guides",
      "links": [
        {
          "kind": "wiki",
          "id": "leather-from-hides",
          "label": "Leather from hides"
        },
        {
          "kind": "wiki",
          "id": "backpack-upgrades",
          "label": "Backpack upgrades"
        },
        {
          "kind": "wiki",
          "id": "grizzly-bear-guide",
          "label": "Grizzly Bear and Heavy Hide"
        }
      ]
    }
  ]
}
```

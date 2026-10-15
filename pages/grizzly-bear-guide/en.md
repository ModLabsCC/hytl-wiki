---
hytlMarkdown: 1
locale: en
title: Grizzly Bear
slug: creatures/grizzly-bear
description: The Grizzly Bear is a source of Heavy Hide and raw wildmeat in the
  release drop records. Heavy Hide is the raw material to follow when a recipe
  asks for Heavy Leather.
status: complete
sources:
  - url: https://hytl.dev/entities/Bear_Grizzly
    title: Grizzly Bear
    revision: sha256:54a45f551304802c977a9eb1f38f63b102a5533119b6fb44cda5f305c83a13b1
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
  - url: https://hytl.dev/items/Ingredient_Hide_Heavy
    title: Heavy Hide
    revision: sha256:3072d9dd02900631abaaaed3cab713ae900ab63d2065ecf09d95b528598d86ea
    retrievedAt: 2026-10-15T13:44:32.669108+00:00
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    modifications: Original editorial explanation. Current live components may show
      later indexed values.
---

The Grizzly Bear is a source of Heavy Hide and raw wildmeat in the release drop records. Heavy Hide is the raw material to follow when a recipe asks for Heavy Leather.

```hytl:creature
{
  "entity": "Bear_Grizzly"
}
```

## Drops to gather

```hytl:drops
{
  "entity": "Bear_Grizzly"
}
```

Check the material name before hunting. Medium Hide will not satisfy a Heavy Hide ingredient merely because both are hides. Once you have the right raw material, follow the :wiki[leather-processing guide]{page="leather-from-hides"} for the corresponding Tanning Rack recipe.

## Read the bear's configured behaviour

The observed role identifies the Grizzly Bear as a memory-bearing creature in the Predator category. Its behaviour configuration uses a roar for the threaten animation and contains separate stomp and left/right swipe damage interactions.

These distinct interactions are why a single “damage” number would be misleading without attack context. The role's raw fields are available through the creature record for readers who need the exact configuration.

```hytl:data-values
{
  "type": "entity",
  "id": "Bear_Grizzly"
}
```

## Finding one

The observed Grizzly Bear detail record does not contain a spawn-region list. This page therefore does not turn the bear's name, colour or an old promotional image into a verified biome location. Use a confirmed sighting in your world or later indexed spawn data to narrow the search.

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
          "id": "medium-hide-sources",
          "label": "Medium Hide sources"
        },
        {
          "kind": "wiki",
          "id": "memories-and-heart",
          "label": "Memories"
        }
      ]
    }
  ]
}
```

---
hytlMarkdown: 1
locale: en
title: Leather from hides
slug: materials/leather-from-hides
description: Distinguish Light, Medium and Heavy Hide from processed leather,
  and follow the recorded sources and processing recipes.
status: complete
sources:
  - url: https://hytl.dev/items/Ingredient_Leather_Light
    revision: sha256:8a9f62ce9c1495af6f8af64406bb2e14f64cd6faa45f8a4bab983a30097b7fa0
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Light Leather
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Leather_Medium
    revision: sha256:02173d33b2316a6b0f09ea7f9f4f55bcaef60476181603d3b9620377cf456cd6
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Medium Leather
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Leather_Heavy
    revision: sha256:23b48a5a555d86903fdd0719e80bdea3f6650c07c09f80bf1404977618d2ccf7
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Heavy Leather
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Hide_Light
    revision: sha256:070d276f2666fd6a603f145403c594dfae0cb58c75f6f6fed528dbb914c433ac
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Light Hide
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Hide_Medium
    revision: sha256:8be9aa9b3625bf714a8f74d6f274ae3e08cfd7637fae2c708b6f52794ef29063
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Medium Hide
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Hide_Heavy
    revision: sha256:71b225ac0aa118841db3993b1d9286b60fff1a4642e9e6ff0ff390a4401dbb5e
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Heavy Hide
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
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

## Look for the raw material first

A request for leather can mean two different things: finding the raw hide or processing it into the leather required by a recipe. Decorative objects with “leather” in their name answer neither question. Match the ingredient record before planning what to gather.

The release index has separate records for :item[Light Hide]{id="Ingredient_Hide_Light"}, :item[Medium Hide]{id="Ingredient_Hide_Medium"} and :item[Heavy Hide]{id="Ingredient_Hide_Heavy"}. Their item pages list recorded creature-drop sources. Those source lists identify where the data connects a material to a creature; they do not by themselves establish a guaranteed drop on every kill.

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/e750c7bdc4c84ae4fc045b979203ea416a2e51f51eee2399dc6170d12e9beb53.png",
      "alt": "A group of camels walking across a dry landscape at sunset.",
      "caption": "Camels in an official development screenshot. When gathering hides, consult the current material source lists rather than assuming a drop from an animal illustration. Work in progress; the final game may differ.",
      "source": {
        "url": "https://cdn.hytale.com/5e7b9ecb50cbcd001176c5c1_11___z2_camels.png",
        "title": "Camels — official Hytale screenshot",
        "revision": "sha256:634373462011c362c23f04561aefc3591346df294f8b64a1a8880f16c1ae9735",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.781Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: e750c7bdc4c84ae4fc045b979203ea416a2e51f51eee2399dc6170d12e9beb53"
      }
    }
  ]
}
```

## Process the matching hide

Light, Medium and Heavy Leather each have their own processing recipe. Open the recipe for the leather your finished item actually requires. Similar names do not make the three materials interchangeable.

::recipe{item="Ingredient_Leather_Light"}

::recipe{item="Ingredient_Leather_Medium"}

::recipe{item="Ingredient_Leather_Heavy"}

## Continue to the finished item

Once you have the required leather, follow its uses or return to your target recipe. The :wiki[Iron Sword guide]{page="crafting-an-iron-sword"} is one example of a chain that includes processed leather as well as metal.

This article describes the relationship between records. The live recipe cards show current indexed inputs and processing requirements; the source section records the revision used for the explanation.

---
hytlMarkdown: 1
locale: en
title: Crafting an Iron Sword
slug: crafting/an-iron-sword
description: Trace the Iron Sword recipe through its metal and leather
  ingredients without mixing up finished materials and raw resources.
status: complete
sources:
  - url: https://hytl.dev/items/Weapon_Sword_Iron
    revision: sha256:f353a19b2b3fbc0aa7fc4ab6496ba0c6c08b576019476d64c5c8791746675ef6
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Iron Sword
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Bar_Iron
    revision: sha256:a6ceb2aba94b1182fd51cdbca6add703e56d828c4fa3071c1a4d7bff0285943e
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Iron Ingot
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
  - url: https://hytl.dev/items/Ingredient_Leather_Light
    revision: sha256:8a9f62ce9c1495af6f8af64406bb2e14f64cd6faa45f8a4bab983a30097b7fa0
    license: Factual game-data reference; Hytale assets retain their original
      rights. No source prose or media reproduced.
    retrievedAt: 2026-10-15T08:59:52.927Z
    attribution: Hytale game-file records, observed in the HYTL.DEV release index
    title: Light Leather
    modifications: Independently authored explanation of observed facts. Live
      components may show newer indexed values.
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

## Begin with the finished recipe

:item[Iron Sword]{id="Weapon_Sword_Iron"} is the finished item. Its recipe identifies the required ingredients and workstation. Use that recipe as the checklist: a related resource name is not a substitute for the exact input named by the game record.

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/1b71029ca48e06e4ea226ad0e597954dcca93a612a30a4b8a38bfaeb0776c626.png",
      "alt": "A red-haired player holding a sword beside a workbench in a wooden workshop.",
      "caption": "A sword beside a workbench in an official development screenshot. Use the live recipe below for current Iron Sword ingredients and workstation requirements. Work in progress; the final game may differ.",
      "source": {
        "url": "https://cdn.hytale.com/5e7ba29b50cbcd001176c699_83___crafted_sword.jpg",
        "title": "Crafted sword — official Hytale screenshot",
        "revision": "sha256:66fb21aeef7af480622f5ae897ec0b6eaef4dc2bf17446ff4b55d7712cf31178",
        "license": "Hytale editorial media permission (Content Creators FAQ); copyright retained by Hypixel Studios. Not CC BY.",
        "retrievedAt": "2026-10-15T12:48:49.684Z",
        "attribution": "© Hytale / Hypixel Studios. Official development screenshot; no endorsement implied.",
        "modifications": "Resized proportionally to 1600 × 900; re-encoded as PNG with metadata removed. No crop or compositing. Asset SHA256: 1b71029ca48e06e4ea226ad0e597954dcca93a612a30a4b8a38bfaeb0776c626"
      }
    }
  ]
}
```

::recipe{item="Weapon_Sword_Iron"}

## Prepare the metal

:item[Iron Ingot]{id="Ingredient_Bar_Iron"} is a processed ingredient. Follow its recipe to the ore input and processing station. This separates the gathering step from the final equipment craft and avoids counting ore as ready-to-use ingots.

::recipe{item="Ingredient_Bar_Iron"}

## Prepare the leather

The sword's observed release recipe also references :item[Light Leather]{id="Ingredient_Leather_Light"}. Light Leather and Light Hide are separate records. Read :wiki[Leather from hides]{page="leather-from-hides"} for the raw-material chain, then return to the sword recipe for its exact requirements.

## Check quantities in the live recipe

The component above shows the indexed requirements instead of freezing a second table in this guide. If the game changes the recipe, compare the component's data context with the article's recorded source. A listed crafting duration does not establish a weapon's attack speed or damage per second.

::data-values{type="item" id="Weapon_Sword_Iron"}

---
hytlMarkdown: 1
locale: en
title: "Chapter I: where to start"
slug: exploration/chapter-one
description: "Find the Goblin Lab, restore its power, and follow the chapter objectives. A separate spoiler guide covers lab upgrades and The Deepworks."
status: complete
sources:
  - {"url": "https://hytale.com/news/2026/10/2026-10-12-chapter-i-out-of-the-breach/", "revision": "sha256:c8332f4800d7c6eb17e4d70856bbd02c87421fbd9fe2f57fd9c3917c13e93257", "retrievedAt": "2026-10-15T14:40:52.850Z", "title": "Chapter I: Out of the Breach", "license": "Factual reference to official Hytale release notes; independently written summary, no copied article.", "attribution": "Hytale Team / Hypixel Studios", "modifications": "Selective summary. Lab costs and recipe requirements are independently checked against release game records."}
  - {"url": "https://hytl.dev/items/GoblinLab_Generator", "title": "Goblin Power Generator", "revision": "sha256:95b1d2917b3cdf115af7ea802cc2a5de4acfdd097173cec96623f93595cb9455", "retrievedAt": "2026-10-15T14:42:46.022603+00:00", "license": "Factual game-data reference; Hytale assets retain their original rights. No source prose reproduced.", "attribution": "Hytale release game-file records, checked against the HYTL.DEV release index", "modifications": "Original explanation and repair-cost tables from AugmentBlock upgrades; crafting requirements from the actual recipe."}
  - {"url": "https://hytl.dev/wiki/exploration/chapter-one", "title": "Hytale2026-10-15_16-12-25.png", "revision": "sha256:dcc488afb79b022140147b9eee27d29da95e4ddbbed171fb16fde7e67b0ebb10", "retrievedAt": "2026-10-15T14:42:46.022603+00:00", "license": "Contributor-supplied gameplay screenshot, supplied for publication in this wiki. Hytale assets retain their original rights; excluded from the article text license.", "attribution": "Community gameplay screenshot · Hytale assets © Hypixel Studios.", "modifications": "Proportional resize from 3840×2160 to 1600×900; metadata-free canonical PNG. No crop, compositing or generated artwork."}
---

**Chapter I: Out of the Breach** arrived in Exploration Mode on **12 October 2026**. Start at the Forgotten Temple; existing worlds and new saves are supported.

```hytl:zone-hero
{
  "zone": "ForgottenTemple"
}
```
## Find the Goblin Lab

Look for the scrap-metal structure built into a temple tower. The entrance in the supplied screenshot has pipes, metal stairs and bright goblin signs against the older stonework.

```hytl:gallery
{
  "media": [
    {
      "type": "image",
      "src": "/wiki-assets/008005c8c21cbc28213f044f30959cda687ff9e6b498174f00241a0cd1d671ae.png",
      "alt": "Scrap-metal entrance built into a vine-covered tower at the Forgotten Temple",
      "caption": "The Goblin Lab entrance at the Forgotten Temple. Community gameplay screenshot, 15 October 2026.",
      "source": {
        "url": "https://hytl.dev/wiki/exploration/chapter-one",
        "title": "Hytale2026-10-15_16-12-25.png",
        "revision": "sha256:dcc488afb79b022140147b9eee27d29da95e4ddbbed171fb16fde7e67b0ebb10",
        "retrievedAt": "2026-10-15T14:42:46.022603+00:00",
        "license": "Contributor-supplied gameplay screenshot, supplied for publication in this wiki. Hytale assets retain their original rights; excluded from the article text license.",
        "attribution": "Community gameplay screenshot · Hytale assets © Hypixel Studios.",
        "modifications": "Proportional resize from 3840×2160 to 1600×900; metadata-free canonical PNG. No crop, compositing or generated artwork."
      }
    }
  ]
}
```
## Restore power

The :item[Goblin Power Generator]{id="GoblinLab_Generator"} has a recorded repair cost of **10 Scraps**. Gather :item[Scraps]{id="Ingredient_Scraps"}, interact with the generator and check its repair prompt. Power is also a prerequisite for the lab's other recorded repairs and recipes.

```hytl:infobox
{
  "type": "item",
  "id": "GoblinLab_Generator"
}
```
Use the **Chapter screen** to follow your current objective and its unlock. Repair requirements are tied to individual lab machines; a workbench recipe and a machine repair are different interactions.

## Your first breach

A temporary Goblin Breach leads to a regenerating fragment of Orbis. Void pressure eventually ends the visit; fighting it and upgrading the lab's Breach Console can buy more time. Return to the lab as you collect materials.

## Continue with spoilers

:::callout{kind="warning" title="Progression and dungeon spoilers"}
The :wiki[Goblin Lab and Deepworks guide]{page="goblin-lab-guide"} contains interior screenshots, repair costs, fragment recipes and boss names. Open it when you want the next steps explained.
:::

```hytl:navbox
{
  "title": "Keep exploring",
  "groups": [
    {
      "title": "Guides",
      "links": [
        {
          "kind": "wiki",
          "id": "goblin-lab-guide",
          "label": "Goblin Lab and Deepworks — spoilers"
        },
        {
          "kind": "wiki",
          "id": "backpack-upgrades",
          "label": "Backpack upgrades"
        },
        {
          "kind": "wiki",
          "id": "repair-kits-guide",
          "label": "Repair kits"
        },
        {
          "kind": "wiki",
          "id": "exploration-field-guide",
          "label": "Exploration field guide"
        }
      ]
    }
  ]
}
```

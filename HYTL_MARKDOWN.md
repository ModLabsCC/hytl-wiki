# HYTL Markdown 1 — public format specification

HYTL Markdown is GFM, YAML frontmatter and a fixed registry of data directives.
It is not MDX: HTML, JSX, imports, executable templates and unknown directives
are rejected. Code examples and escaped directives remain ordinary Markdown.
GitHub does not render HYTL components. Use the authenticated HYTL editor preview
or the trusted standalone validator; do not run programs supplied by an article.
The core and this specification are MIT licensed; this grants no rights to
articles, media, game assets or private HYTL application code.

## Article metadata

```yaml
---
hytlMarkdown: 1
locale: en
title: An original guide
slug: guides/original-guide
description: What this guide covers.
status: stub
aliases: [old-original-guide]
---
```

Published articles require frontmatter. Plain Markdown without frontmatter is
valid in the core preview. Status is `stub`, `outdated`, `work-in-progress` or
`complete`; it never grants publication rights. Translation frontmatter also
requires `sourceLocale` and the source article's 64-character SHA-256
`sourceRevision`. See [the content schema](content-schema.md) for shared metadata,
taxonomy, source records and revisions. Unknown fields are errors, including
free-form author identities.

## Syntax

Inline references have one colon and a text label:

```md
:item[Iron]{id="VERIFIED_ITEM_ID"}
:entity[Creature]{id="VERIFIED_ENTITY_ID"}
:zone[Zone]{id="VERIFIED_ZONE_ID"}
:wiki[Crafting]{page="stable-page-id"}
:site-page[Crafting]{id="crafting"}
```

Reference labels are normal inline Markdown. Page IDs do not change with title,
slug or locale. IDs in this document are placeholders; choose verified IDs in
the editor. `site-page` IDs come from a fixed application registry (`home`,
`items`, `blocks`, `entities`, `zones`, `crafting`, `updates`, `wiki`).

Blocks have two colons. They do not accept an inline label:

```md
::infobox{type="item" id="VERIFIED_ITEM_ID"}
::recipe{item="VERIFIED_ITEM_ID"}
::drops{entity="VERIFIED_ENTITY_ID"}
```

Editorial containers have three colons and preserve nested Markdown:

```md
:::callout{kind="warning" title="Check the version"}
This is **editorial text**, with :item[an item]{id="VERIFIED_ITEM_ID"}.
:::
```

`callout` accepts `note` (default), `tip`, `info`, `warning`, `danger`. Other
editorial containers are listed below. Structured properties use strict JSON
data fences, normalized to exactly the same nodes as directives:

````md
```hytl:weapon-compare
{"items":["VERIFIED_WEAPON_A","VERIFIED_WEAPON_B"]}
```
````

Only `hytl:recipe` additionally accepts one bare item ID. No other heuristic text
interpretation exists. Ordinary fences such as `md` or `json` always remain
code. Container content belongs in a container, not in a data fence. An inline
reference written with two colons is an error rather than an alternative syntax.

## Registry

All entries support Markdown 1. Unless indicated, components support block and
JSON-fence syntax. `?` indicates an optional prop. All unlisted props are errors.
`id` is a bounded game ID; `source` is the full validated provenance object.
The executable registry exports strict Zod `propsSchema`, allowed forms,
renderer key, data requirements, context, reference extractor, capabilities,
editor label/description/snippet and missing-data behavior. Editor forms and
autocomplete consume it directly; they do not maintain a second grammar.

| Name | Properties | References/data behavior |
| --- | --- | --- |
| `infobox` | `type:item/entity/zone`, `id`, `title?` | Explicit object |
| `recipe` | `item` | Explicit item; defined crafting recipe |
| `salvage` | `item` | Defined salvage only; never reversed crafting |
| `recipe-book` | `bench?`, `category?`, `page`, `limit` | Only bench is an explicit reference; result pages do not expand the graph |
| `bench-ladder` | `bench`, `source?` | Bench; container also allowed |
| `drops` | `entity` | Creature; extracted drops |
| `loot` | `id`, `type:item/entity` (default item) | Explicit object; weights are not probabilities |
| `ore-map`, `zone-bars` | `item`, `zones?` | Item and explicitly selected zones |
| `tier-progression` | `items`, `source?` | Explicit items; container also allowed; no inferred tiers |
| `weapon-compare` | `items` | Comparable extracted weapon values; no inferred DPS |
| `attacks` | `entity` | Extracted creature attacks |
| `creature` | `entity` | Creature card |
| `creature-grid` | `entities?`, `zone?`, `faction?`, `page`, `limit` | Explicit creatures/zone; dynamic results do not expand the graph |
| `zone-hero` | `zone`, `title?` | Zone banner |
| `regions` | `zone` | Extracted region connections |
| `faction` | `id`, `title?`, `source?` | Editorial container also allowed; no invented lifecycle |
| `furniture-set` | `items`, `title?` | Explicit items |
| `memories` | `id`, `source?`, `tracker` (default false) | Editorial container also allowed; optional tracker is browser-local |
| `crop` | `item`, `source?` | Item; editorial container also allowed; missing timings stay unknown |
| `data-values` | `type:item/entity/zone`, `id` | Explicit object; IDs/variants |
| `history` | `page?`, `entries?:[{date,text,source}]` | Editorial container also allowed; no invented authors/game versions |
| `gallery` | `media:[image/video]` | Approved content-addressed image assets; restricted video URLs |
| `navbox` | `title`, `groups:[{title,links:[{kind,id,label?}]}]` | Explicit related references |
| `status` | `status?` | Validated editorial metadata only |
| `hub-tiles` | `pages?`, `tag?`, `category?`, `page`, `limit` | Explicit pages only; dynamic results do not expand the graph |
| `callout` | `kind`, `title?` | Container only; nested editorial Markdown |
| `item`, `entity`, `zone`, `site-page`, `asset` | `id` | Inline mention only |
| `wiki` | `page` | Inline mention only |

Pagination defaults to page 1, limit 12; maximum page 10,000 and limit 50.
Explicit comparison/object arrays contain at most 24 IDs. All live components
require host-provided `locale`, `patchline` and `datasetGeneration`; content
cannot supply an arbitrary URL, class, style, handler, SQL or search expression.
Missing live objects/fields render a localized partial/unavailable state and do
not hide the surrounding article. The renderer adapter determines actual data
capabilities, described separately in the private integration capability report.
The compiler validates syntax and references, never claims that a game ID exists
without catalog validation by the publisher.

## Images and links

Markdown images and gallery images must use
`/wiki-assets/<64-character-sha256>.<png|jpg|jpeg|webp|gif|avif>`. Gallery images
require `alt`, optional `caption` and optional `source`. The matching binary file
must exist in `assets/`. External images, SVG, HTML and data URLs are rejected.
Approved assets pass a trusted decoding/sanitization pipeline before upload.
Compiler image checks verify filename hash, signature and dimensions; they are
not a replacement for a full image decoder or legal rights review.

Gallery video records require `type:"video"`, `src`, `title`, optional `caption`
and a full `source`. Supported URLs are HTTPS
`www.youtube-nocookie.com/embed/<11-character-id>` and
`player.vimeo.com/video/<numeric-id>`. No autoplay/query parameters or arbitrary
iframes are accepted.

Links allow HTTPS (without credentials), same-document safe anchors, controlled
game detail routes and localized wiki article routes. Other schemes, protocol
relative URLs, backslashes, traversal, control characters and arbitrary internal
application paths are errors. Prefer `:wiki` references over hardcoded slugs.
Explicit wiki URLs must resolve in the candidate snapshot. Item/creature/zone
links also contribute mention references to the backlink graph.

## Headings, limits and serialization

Headings receive Unicode-aware IDs; repeated generated IDs append `-2`, `-3`.
An explicit trailing `{#safe-anchor}` uses Unicode letters/numbers, hyphens and
underscores. Duplicate explicit anchors and missing local link anchors fail
validation. The same AST supplies the renderer, table of contents and search.

Central limits: article 256 KiB UTF-8, frontmatter 24 KiB, AST depth 40, 20,000
AST nodes, 100 embeds, 16 KiB component props, 500 table data rows, 50 media
objects. Snapshot limits are 25,000 files and 64 MiB encoded content. Raster
assets are bounded to 12 MiB base64 input, 8,192 pixels per side and 32 million
pixels. Oversized input is reported, never silently truncated and published.

`compileMarkdown(text,{path?,locale?})` returns protocol/compiler/registry
versions, validated frontmatter, plain JSON mdast, headings, typed references,
deduplicated live requirements, links, plain text and positioned diagnostics.
Normalized nodes are `hytlEmbed` and `hytlReference` from the integration
contract. `serializeMarkdown(result)` uses maintained GFM/directive serializers,
preserves approved fields and rejects invalid content. Formatting may change;
unknown fields are never silently discarded.

Editor forms use `readFrontmatter(markdown)` to read raw metadata even when
known fields are temporarily incomplete. It returns null when metadata is
absent and throws on malformed YAML. `updateFrontmatter(markdown,patch)` is
strict by default and preserves the raw body byte-for-byte. Its editor-only
`{validate:false}` option permits incomplete known values while typing; it
still rejects unknown keys and does not certify publication. The normal
compiler validates every candidate before submit/publish.

## Trusted CLI

Build with `node scripts/build-wiki-compiler.mjs` in the private application.
The standalone `dist/wiki-compiler/cli.mjs` contains the neutral core and its
dependencies, never the React application, runner, credentials or content repo
programs. Node 24 reads exactly one bounded UTF-8 JSON stdin document:

```json
{"protocolVersion":1,"command":"compile","markdown":"# Example","locale":"en"}
```

`command:"snapshot"` instead receives `files`, `commit`, `repo`, `branch` and
`createdAt` as documented in the content schema. Output is one JSON document.
Exit 0 is transport success; check `ok` for content validity. Invalid transport
exits 2. The runner limits process runtime, output and concurrency. No network
is performed by the compiler, and no program from the article repository runs.

The browser and Worker import the same core. Workers resolve the dependency
condition `worker`/`workerd`/`edge-light`; this selects pure entity decoding
without a DOM. Tests compare Node, bundled CLI and a DOM-free Worker bundle.

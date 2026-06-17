# Compatibility

## Gravewright compatibility

This package targets:

```text
Gravewright: 2.0.0-alpha.0+
SDK: 1
```

Manifest compatibility:

```json
{
  "minimum": "2.0.0-alpha.0",
  "verified": "2.0.0-alpha.0",
  "maximum": "2.x"
}
```

## Package kind

```json
{
  "kind": "ruleset",
  "activation": {
    "scope": "campaign",
    "mode": "exclusive"
  }
}
```

A campaign should normally activate only one ruleset.

## SDK capabilities

The package declares:

```text
actors.register
items.register
sheets.declarative
sheets.runtime
rules.declarative
content.packs
tokens.mappings
dice.roll
chat.cards
rolls.intent
locales
assets.ui
assets.styles
assets.scripts
combat.config
combat.runtime
```

## Package path

Expected local path:

```text
data/packages/rulesets/dnd5e
```

## Compatibility scope

This package is intended as a 5e/SRD-compatible framework. It does not guarantee
feature parity with every official or third-party 5e product.

## Breaking changes

Breaking changes should be documented in `CHANGELOG.md`.

Examples of breaking changes:

- actor schema field removal or rename;
- item schema field removal or rename;
- content pack ID rename;
- actor/item type ID rename;
- package ID rename;
- capability removal;
- sheet path rename;
- rule formula ID rename.

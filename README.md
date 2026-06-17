# 5e SRD Compatible Framework for Gravewright

Unofficial 5e/SRD-compatible ruleset package for Gravewright.

This package provides schemas, sheets, rules, mappings, automation, and small
sample/model content packs for running 5e-compatible games in Gravewright. It is
designed as a technical ruleset framework, not as a replacement for any official
rulebook or digital compendium.

## Status

Package status: **Alpha / SDK 1 compatible**

Tested with:

```text
Gravewright 2.0.0-alpha.0
SDK 1
```

## What this package includes

- Actor schemas for characters and monsters.
- Item schemas for weapons, armor, equipment, consumables, spells, feats,
  features, races, backgrounds, classes, and effects.
- Declarative actor and item sheets.
- Runtime sheet helpers through `sheets.runtime`.
- Combat panel/runtime integration through `combat.runtime`.
- Dice, roll intent, chat-card, token, and combat mappings.
- Small sample/model content packs for development and drag/drop testing.

## What this package does not include

This package does **not** include:

- official rulebooks;
- official PDFs;
- official artwork;
- official trade dress;
- a full proprietary compendium;
- closed/proprietary monsters, settings, subclasses, spells, or other material
  outside material the project is permitted to use;
- any claim of official affiliation, endorsement, or approval by Wizards of the
  Coast.

Users are responsible for owning and using any rulebooks or content required for
their own table.

## Legal and attribution notice

This is an unofficial compatibility package. See [`NOTICE.md`](NOTICE.md) and
[`CONTENT_POLICY.md`](CONTENT_POLICY.md) before adding content.

Where SRD material is included or adapted, it is attributed under Creative
Commons Attribution 4.0 International (CC BY 4.0). See [`NOTICE.md`](NOTICE.md).

## Installation

See [`INSTALL.md`](INSTALL.md).

Quick install from a Gravewright checkout:

```bash
mkdir -p data/packages/rulesets
git clone https://github.com/Gravewright/gravewright-5e-srd.git data/packages/rulesets/dnd5e
uv run python -m app.cli package validate data/packages/rulesets/dnd5e
uv run python -m app.cli package install dnd5e --enable
uv run python -m app.cli doctor
```

On Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force data\packages\rulesets | Out-Null
git clone https://github.com/Gravewright/gravewright-5e-srd.git data\packages\rulesets\dnd5e
uv run python -m app.cli package validate data/packages/rulesets/dnd5e
uv run python -m app.cli package install dnd5e --enable
uv run python -m app.cli doctor
```

## Repository layout

```text
manifest.json
assets/
content/
layouts/
locales/
mappings/
rules/
schemas/
```

## Compatibility

See [`COMPATIBILITY.md`](COMPATIBILITY.md).

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Security

See [`SECURITY.md`](SECURITY.md).

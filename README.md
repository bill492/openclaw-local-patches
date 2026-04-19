# OpenClaw Local Patches

Canonical Markdown references for the local OpenClaw overrides currently maintained outside upstream.

## Included Patches

- [OV-011](docs/ov-011.md)
- [OV-013](docs/ov-013.md)
- [OV-014](docs/ov-014.md)
- [OV-015](docs/ov-015.md)
- [OV-016](docs/ov-016.md)
- [OV-017](docs/ov-017.md)

## Purpose

This repository is meant to be handed to another Codex session or operator when patching another OpenClaw install.

Each document explains:

- why the override exists
- what behavior it changes
- how to patch the active dist bundle on the matching OpenClaw install version
- how to verify the patch after restart

## Usage

On another install:

1. Identify the active hashed dist bundle for the target module.
2. Apply the patch described in the relevant `docs/ov-*.md` file.
3. Restart the gateway.
4. Verify the live bundle contains the expected markers and behavior.

## Notes

- The bundle hashes in the docs are from Bill's Valhalla install and are examples, not stable upstream identifiers.
- These docs intentionally describe local reimplementations against live dist bundles.

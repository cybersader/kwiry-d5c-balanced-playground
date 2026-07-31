# Kwiry D5C Balanced Playground

Private, fixture-only field-test channel for Kwiry's experimental Balanced ranking playground.

This is **not** the production Kwiry plugin. It uses the distinct Obsidian plugin ID `kwiry-d5c-balanced-playground`, does not connect to live Google Docs or Canva sources, does not change the public/default relevance profile, and does not imply owner acceptance of Balanced ranking.

## Install with BRAT

1. Use a disposable Obsidian vault.
2. Install and enable BRAT.
3. Run **BRAT: Plugins: Add a beta plugin for testing (with or without version)**.
4. Enter `cybersader/kwiry-d5c-balanced-playground`.
5. Select the requested frozen release, initially `0.0.1`.
6. Confirm Obsidian lists **Kwiry D5C Balanced Playground**.
7. Run **Kwiry D5C Balanced Playground: Open private D5C Balanced playground**.

The runtime package contains exactly `main.js`, `manifest.json`, and `styles.css`. Verify their SHA-256 values against the release attestation before testing.

## Source and evidence

Corresponding source for release `0.0.1`:

- repository: <https://github.com/cybersader/kwiry>
- source tag: [`d5c-balanced-playground-0.0.1-source`](https://github.com/cybersader/kwiry/tree/d5c-balanced-playground-0.0.1-source)
- source commit: `ac7b0a0555dedda5e945998e1ad5d776ae297082`

Each frozen release provides the three runtime files plus GPL/Apache notices, `SHA256SUMS`, and a sanitized build attestation. The attestation records source identity, deterministic-build state, embedded artifact identities, cache isolation, and known limitations without vault paths, note content, query content, or credentials.

## Test boundary

Evaluate Text versus strict Balanced ordering, neutralized counterfactual labeling, fatal refusal behavior, explanation levels, bounded property packs, restart/offline behavior, co-installation with production Kwiry, update/rollback, and absence of vault/cache mutation.

The separate production 10,000-note/50-MiB Worker capacity regression is not evaluated by this fixture playground.

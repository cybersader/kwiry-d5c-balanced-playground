# Kwiry D5C Balanced Playground

BRAT field-test channel for Kwiry's experimental local active-vault Text-versus-Balanced search.

This is **not** the production Kwiry plugin. It uses the distinct Obsidian plugin ID `kwiry-d5c-balanced-playground`, does not connect to Google Docs or Canva, does not change the production/default relevance profile, and does not imply owner acceptance of Balanced ranking.

The `0.0.2` owner build reads Markdown from the active disposable vault while enabled. It uses one in-memory local Worker and compiles out daemon access, network access, credentials, settings profiles, and disk-cache persistence. Its index is discarded on unload and rebuilt after restart.

## Install or update with BRAT

1. Use a disposable Obsidian vault.
2. Install and enable BRAT.
3. Run **BRAT: Plugins: Add a beta plugin for testing (with or without version)**.
4. Enter `cybersader/kwiry-d5c-balanced-playground`.
5. Select release `0.0.2`.
6. Confirm Obsidian lists **Kwiry D5C Balanced Playground**, not the normal **Kwiry Search** plugin.
7. Run **Kwiry D5C Balanced Playground: Open Text vs Balanced search**.

The installed plugin directory contains exactly `main.js`, `manifest.json`, and `styles.css`. Verify their SHA-256 values against the release attestation before testing.

Release `0.0.1` remains frozen as the previous fixture-only build for rollback comparison.

## Source and evidence

Corresponding source for release `0.0.2`:

- repository: <https://github.com/cybersader/kwiry>
- source tag: [`d5c-balanced-playground-0.0.2-r6-source`](https://github.com/cybersader/kwiry/tree/d5c-balanced-playground-0.0.2-r6-source)
- source commit: `cb9a28705479423ae311f7578dea62c98a0b777d`

Release `0.0.2` provides the three runtime files plus GPL, Apache-2.0, Emscripten, and exact Rust dependency license terms; third-party notices; `SHA256SUMS`; and a sanitized build attestation. The attestation records source identity, same-environment repeatability, embedded artifact identities, cache/network isolation, and known limitations without vault paths, note content, query content, or credentials.

## What to evaluate

Create recognizable notes in the disposable vault, including a clearly stronger text match, recent and older tied matches, a note under `reference/`, and a note under `archive/`. Then verify:

1. Cold indexing reports a concise count and percentage without question marks.
2. Search becomes available after acknowledged initial batches, with partial coverage labeled honestly.
3. Results show recognizable titles, paths/headings, and snippets and open the intended note or heading.
4. **Text** preserves lexical ordering.
5. **Balanced preview** only reorders equally strong text matches; weaker text never crosses stronger text.
6. Final publication changes partial coverage to complete or honestly incomplete coverage.
7. Restart, offline use, disable/re-enable, update, rollback, and co-installation with production Kwiry do not alter the production cache or leave orphan work.
8. **Copy technical summary** exports aggregate counts and allowlisted failure categories only.

The separate production 10,000-note/50-MiB Worker capacity regression remains unresolved and is tracked outside this field experiment. Release `0.0.2` must report existing limits honestly; it does not fix or bypass that regression.

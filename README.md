# terma-prices

This repository hosts the live price-feed data for [terma](https://github.com/termasubscription), a personal cost & document manager.

## What this is

`catalog.v1.json` is a diff-only overlay of subscription/contract prices, keyed by catalog entry and plan. The terma app fetches this file at runtime and merges it on top of its own bundled catalog. That means price corrections and new brands can reach every running copy of the app immediately, without an app update or rebuild.

The app only ever reads this file - nothing here is executed, and nothing here can act as anything other than data.

## How it's used

- The app calls `feedUrl()` to resolve where to fetch the current feed from, then merges the result over its built-in catalog (`mergeCatalog()`), overriding matching prices and adding any new entries.
- If this file is unreachable or malformed, the app silently keeps using its bundled catalog - a broken or stale feed never breaks the app itself.
- Prices are checked periodically (currently semi-automated, with manual verification against provider websites) and pushed here as small, reviewable diffs.

## License

See [LICENSE](LICENSE). The compiled dataset (selection, structure, categorisation) is all-rights-reserved; the underlying factual prices themselves are not and cannot be copyrighted. This repo is meant to be fetched at runtime by the terma app, not redistributed or reused as a standalone dataset.

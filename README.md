# Audia Distribution

Public Sparkle distribution repository for Audia.

## What lives here

- `appcast.xml` on `main`
- GitHub Release assets (`Audia-<version>.zip`) attached to release tags (`v<version>`)

## Release flow

1. Build and sign update archive from private app repo.
2. Upload `Audia-<version>.zip` to GitHub Release tag `v<version>` in this repo.
3. Update `appcast.xml` with a new top `<item>` that points to the uploaded release asset.
4. Commit and push `appcast.xml` to `main`.
5. Validate Sparkle update flow from an older installed version.

## Invariants

- `sparkle:version` must be monotonic (strictly increasing).
- `enclosure length` must match the ZIP byte size exactly.
- `sparkle:edSignature` must match the ZIP exactly.
- Do not rewrite old release tags or replace release assets in-place.

## Rollback strategy

- If a release is bad, publish a newer fixed version with higher `sparkle:version`.
- Avoid mutating historical entries except to fix hard metadata errors.

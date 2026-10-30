# Cindy Linux arm64 build

This private repository contains the source of makecindy/cindy at tag v0.1.121
(commit 727afb1ad6902176e2ec55254154b900c489a998) plus a GitHub Actions
workflow that builds a Linux arm64 `.deb` natively on `ubuntu-24.04-arm`.

- Upstream workflows and Dependabot config were removed; only
  `.github/workflows/build-linux-arm64.yml` runs.
- The sqlite-vec arm64 binary is fetched from upstream Git LFS and verified
  against the pointer's SHA-256 during the build.
- The package is versionless (app version 0.0.0), so in-app updates are disabled.

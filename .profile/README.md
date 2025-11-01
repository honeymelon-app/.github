# Honeymelon 🍈

High-quality, privacy-respecting media tools for macOS. This organization houses the apps, websites, and infrastructure that power Honeymelon’s distribution, updates, and documentation.

## What we build

- **App**: A fast, reliable macOS media converter with first-class H.264/HEVC support and smart presets.
- **Distribution**: Lightweight, low-cost delivery using GitHub Releases, Cloudflare Pages/Workers, and optional license-gated downloads.
- **Documentation**: Versioned user guides aligned with app releases.
- **Legal**: Immutable, versioned public policies.

## Repositories

Public repos will appear here as they are created. Planned split:

- `website` — Marketing site and download page (Cloudflare Pages)
- `docs` — Versioned documentation
- `legal` — Immutable legal pages (versioned by date)
- `updates` — Public Tauri updater manifests
- `download-worker` — Optional Cloudflare Worker for license-gated downloads
- `app-macos` — Tauri app (Apple Silicon)
- `release-workflows` — Reusable GitHub Actions
- `ops` — Operations notes and future IaC

## Downloads and updates

- Stable builds are published via **GitHub Releases** in `app-macos`.
- The app’s auto-updater reads manifests from the `updates` repository:
  - `https://www.honeymelon.app/updates/stable/latest.json`
- Direct download links are exposed on the `website` repository’s download page.

## Pricing and licensing

- Purchases are handled via a third-party provider (e.g., Lemon Squeezy or Paddle) for taxes and receipts.
- License keys unlock Pro features and may be validated periodically by a lightweight API or Worker.

## Documentation

- Latest: `https://docs.honeymelon.app/latest/`
- Versioned: `https://docs.honeymelon.app/<major.minor>/`

## Legal

- Policies are versioned and permanently accessible:
  - Terms of Service: `https://legal.honeymelon.app/tos/<YYYY-MM-DD>/`
  - Privacy Policy: `https://legal.honeymelon.app/privacy/<YYYY-MM-DD>/`
  - EULA: `https://legal.honeymelon.app/eula/<YYYY-MM-DD>/`
  - Third-party notices and attributions are generated from an SBOM at build time.

## Roadmap (high level)

- Short term: public beta, preset library, stable auto-update channel, docs v1.
- Mid term: license-gated downloads, watch folders, beta channel, telemetry opt-in with on-device logs.
- Long term: R2/S3 artifact storage, staged rollouts, enterprise licensing, Windows build evaluation.

## Contributing

We welcome issues and suggestions. Contribution guidelines and a code of conduct will be published as repositories open up:

- Issue reports: clear steps to reproduce, expected vs. actual behavior, and system details.
- Pull requests: focused changes, tests where applicable, and a short rationale.

## Security and responsible disclosure

If you believe you have found a security issue, please report it privately:

- Email: <security@honeymelon.app>
We aim to acknowledge reports within five business days.

## Contact and support

- General inquiries: <info@honeymelon.app>
- Support requests: <support@honeymelon.app>
- News and release notes will be posted in the `website` repository and on the download page.

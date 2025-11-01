# Honeymelon 🍈

Mac-only media tools for Apple Silicon. We build a small, fast, privacy-first converter that “just works” using FFmpeg, Tauri, and Vue.

---

## What we build

**Honeymelon** is a desktop app for macOS (arm64) that converts video, audio, and images with a clean, preset-driven UI. It favors remux-first workflows, re-encoding only when required, and runs FFmpeg out of process for reliability.

- Simple, guided presets instead of complex flags
- Remux when possible; transcode only when needed
- Local processing by default; no media leaves your machine
- Apple Silicon performance with hardware acceleration via VideoToolbox
- Small footprint and fast startup using Tauri

---

## Why it exists

Media converters tend to be either heavyweight or overly technical. Honeymelon aims for a narrow, reliable core:

- Sensible defaults for common tasks
- Minimal UI with strong affordances
- Predictable output compatible with mainstream players and editors

---

## Technology

- **Desktop:** Tauri (Rust) + Vue 3 + Vite + TypeScript + shadcn-vue
- **Engine:** FFmpeg and FFprobe invoked out-of-process
- **Packaging:** macOS Apple Silicon, signed and notarized
- **Updates:** Optional in-app updates with signed feeds

---

## Roadmap (high level)

- v1: Many-to-many conversions, subtitle handling, basic queue, dark mode
- v1.1: Batch folder ingest, simple rename templates, per-track selection
- v1.2: Trim and basic crop when re-encoding, improved telemetry opt-in
- v2: Plugin-style preset packs and enterprise distribution options

---

## Repositories

- `honeymelon` — desktop app (Tauri + Vue)
- `site` — marketing website and downloads
- `docs` — user guide and licensing notes
- `ffmpeg-builds` — reproducible Apple Silicon FFmpeg/FFprobe builds

(Names may change as the organization evolves.)

---

## Contributing

We welcome focused contributions that keep the app small, fast, and easy to use.

1. Open an issue describing the change and its impact on simplicity and performance.
2. Follow our coding standards (TypeScript strict, ESLint + Prettier, minimal Rust).
3. Keep the UI within shadcn-vue components and utility classes. No custom CSS.

Security reports: contact the maintainers directly. We coordinate responsible disclosure.

---

## Legal

Honeymelon uses FFmpeg under the LGPL. We do not enable GPL or non-free components in our distributed builds. Some codecs may be patent-encumbered in certain jurisdictions; we prefer system-provided implementations where applicable. See the app’s Third-Party Notices for details.

---

## Links

- Website: <https://honeymelon.app>
- Documentation: <https://docs.honeymelon.app>
- Issues: <https://github.com/honeymelon-app/honeymelon/issues>
- Releases: <https://github.com/honeymelon-app/honeymelon/releases>

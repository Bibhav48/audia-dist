# Audia

Audia is a native macOS audio command center focused on precision control and low‑latency performance.

Status: Alpha (free trial).

## What’s in this repo

- Public releases (Sparkle appcast + release assets).
- Issue tracking for bugs and feature requests.

## Download

Get the latest build from the Releases page.

## First‑run note (macOS Gatekeeper)

Alpha builds are not notarized, so macOS may warn that Audia is from an unidentified developer. If that happens:

1. Open Applications and find Audia.
2. Right-click (or Control-click) and choose Open.
3. Confirm Open in the prompt.

## Features

- Per‑app volume control and stereo panning.
- Native multi‑device routing without virtual audio drivers.
- 10‑band EQ system‑wide or per‑app.
- Isolated per‑app recording.
- Built‑in ambient soundscapes.
- Minimal “Liquid Glass” HUD.

## System permissions

Per‑app routing and isolated recording require macOS system permissions. Audia will prompt you on first launch. If anything stops working, check System Settings and re‑enable access.

## Compatibility

Verified on macOS 14.x. Earlier versions may work but are not guaranteed during alpha.

<!--
## Known limitations (alpha)

- Some devices may not expose independent channels for routing or capture.
- EQ and routing changes may take a moment to apply after wake or device re‑connect.
- UI polish is still in progress.
-->

## Privacy

Audia does not collect personal data or audio content. Crash reports, if enabled by you, include technical diagnostics only.

## Feedback and bugs

This is the public hub for releases and issue tracking. If you see a crash, bug, or missing feature, open a new issue.

Please include:

- macOS version.
- Audia version.
- Steps to reproduce.

## Status and roadmap

Audia is in active development by Bibhav Adhikari and Arjav Lamsal. The current v0.2.x series is a free‑trial alpha. A full release and official website are planned.

# OpenNovaLauncher

> Open reverse-engineering, de-bloat, and preservation workspace for Nova Launcher.

**Version**: `1.0.0`

## Overview

OpenNovaLauncher is a research and preservation effort focused on analyzing, documenting, and reconstructing core launcher components from Nova Launcher:
- Removal of telemetry and third-party tracking SDKs (Amplitude, etc.)
- Analysis of paywall mechanisms (`NovaPaywallActivity`)
- Clean isolation of essential desktop management components (`Workspace`, `Folder`, `FolderIcon`, `NovaLauncher`)

## Repository Structure

```
├── re/
│   ├── nova.apk          # Reference base APK
│   ├── nova-src/         # JADX decompiled sources
│   ├── nova-src2/        # Alternative decompile pass
│   └── single/           # Isolated core components for inspection
│       ├── NovaLauncher.java
│       ├── NovaApplication.java
│       ├── NovaPaywallActivity.java
│       ├── Workspace.java
│       ├── Folder.java
│       └── FolderIcon.java
└── README.md
```

## Milestone v1.0.0

- [x] Base APK acquisition and JADX decompile pipeline setup.
- [x] Extraction and isolation of core UI and lifecycle classes.
- [x] Tracking and paywall boundary identification.

## Disclaimer

This repository is for educational, interoperability, and software preservation purposes under applicable reverse-engineering fair use provisions. All original trademarks belong to their respective owners.

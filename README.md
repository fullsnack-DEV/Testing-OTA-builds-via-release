# Testing OTA builds via release

This repo hosts OTA (over-the-air) update files for a React Native app. The app requests these URLs:

- `https://raw.githubusercontent.com/fullsnack-DEV/Testing-OTA-builds-via-release/main/version.txt`
- `https://raw.githubusercontent.com/fullsnack-DEV/Testing-OTA-builds-via-release/main/bundle.zip`

## Requirements

1. **Repo root on `main`** — For the raw URLs to work, this repo **must** have both `version.txt` and `bundle.zip` at the **repo root** on the `main` branch.

2. **version.txt** — A single line containing only the OTA version string (e.g. `1.0.4`). No extra text or newlines.

3. **bundle.zip** — The zip produced by the app’s **build-ota** script. You must add or update `bundle.zip` here after building; do not commit a placeholder — the app needs the real bundle.

# Hardened Browser Profile

This repository provides a **manual hardened browser configuration** designed for
privacy researchers, and penetration testers.

The project does NOT modify your system automatically.
All files must be applied manually by the user.

## Repository contents

- `bookmarks.json`
  Curated bookmark collection (100+ entries) for:
  - anonymity & fingerprint testing
  - IP / ASN / DNS analysis
  - email and phone validation
  - OSINT and reconnaissance
  - exploits and vulnerability research
  - testing playgrounds and privacy resources

- `user.js`
  Hardened Firefox / LibreWolf preferences focused on:
  - fingerprint resistance
  - network isolation
  - WebRTC leak prevention
  - HTTPS enforcement
  - reduced tracking surface

- `theme.xpi`
  Custom browser theme with embedded background image.
  All assets are stored locally inside the extension.
  No remote resources are loaded.

## Supported browsers

- Firefox (latest stable / ESR)
- LibreWolf

## Installation (Manual)

### 1. Install browser
Install Firefox or LibreWolf using your system package manager or official website.

### 2. Import bookmarks
1. Open the browser
2. Bookmarks → Manage Bookmarks
3. Import and Backup → Import Bookmarks from JSON
4. Select `bookmarks.json`

### 3. Add-ons
1. Ublock Origin
2. Decentraleyes
3. LocalCDN
4. User-Agent switcher and manager
5. HTTPS Everywhere
6. FoxyProxy
7. Wappalyzer
8. Dark Reader
9. FlagFox
10. i dont still care about cookies

### 4. Apply hardened preferences
1. Locate your browser profile directory
2. Copy `user.js` into the profile root
3. Restart the browser


Note:
Existing preferences may override or conflict with these settings.

### 4. Install theme
1. Open browser Add-ons manager
2. Install Add-on From File
3. Select `theme.xpi`

## Security notes

- This repository does NOT include malware, telemetry, or auto-update mechanisms
- No scripts are executed
- No system files are modified
- No remote connections are introduced by configuration

## Disclaimer

This configuration improves privacy and research convenience,
but does NOT guarantee anonymity.

Operational security depends on:
- your network setup
- your behavior
- your threat model

Use responsibly.

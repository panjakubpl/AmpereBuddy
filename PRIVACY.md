# Privacy Policy

**Last updated: December 2025**

AmpereBuddy is committed to protecting your privacy. This document explains what data the application collects, how it's used, and how it's stored.

---

## Summary

- **No telemetry or analytics**
- **No user tracking**
- **No cloud sync or accounts**
- **All data stored locally on your Mac**
- **No data shared with third parties**

---

## Data Collection

### What We DO NOT Collect

AmpereBuddy does **not** collect, transmit, or share:

- Personal information (name, email, address)
- Device identifiers or unique IDs
- Location data
- Usage statistics or analytics
- Browsing history
- File system content
- Crash reports (not transmitted externally)
- Any data to third-party services

### What We DO Store Locally

AmpereBuddy stores the following data **only on your Mac**:

#### Battery History (`battery_history.json`)
- Weekly snapshots of battery health
- Data includes: timestamp, health percentage, cycle count, capacity
- Purpose: Track battery degradation over time
- Location: `~/Library/Application Support/AmpereBuddy/`

#### Event Log (`alerts_log.json`)
- Battery-related events (charger connected, low battery, etc.)
- Maximum 500 entries (older entries automatically removed)
- Purpose: Review battery usage patterns
- Location: `~/Library/Application Support/AmpereBuddy/`

#### Error Log (`error.log`)
- Application error messages for troubleshooting
- Maximum 100 KB (auto-rotates)
- Purpose: Debugging issues
- Location: `~/Library/Application Support/AmpereBuddy/`

#### User Preferences
- Display settings, notification preferences, theme selection
- Standard macOS UserDefaults storage
- Location: `~/Library/Preferences/`

---

## Network Access

### Update Checks (Optional)

AmpereBuddy can check for updates from our server:

- **Endpoint**: `macfoundry.it/amperebuddy/downloads/version.json`
- **Method**: HTTPS GET request
- **Data sent**: None (no user information transmitted)
- **Data received**: Version number, release notes, download URL
- **Security**: Certificate pinning + Ed25519 signature verification
- **Frequency**: Every 6 hours (when enabled)
- **Control**: Can be disabled in Settings > System

### No Other Network Activity

The application makes **no other network requests**. All battery monitoring, data storage, and processing happens entirely on your device.

---

## Data Security

### Local Storage
- All data files are stored in your user directory
- Protected by macOS file permissions
- Encrypted if you use FileVault

### Update Verification
- Certificate pinning prevents man-in-the-middle attacks
- Ed25519 cryptographic signatures verify update authenticity
- SHA-256 checksums verify download integrity

---

## Third-Party Services

AmpereBuddy uses **no third-party services**:

- No analytics (Google Analytics, Mixpanel, etc.)
- No crash reporting (Crashlytics, Sentry, etc.)
- No advertising networks
- No social media integration
- No cloud storage providers

The only external dependency is the optional update check to `macfoundry.it`.

---

## Your Rights

### Data Access
All your data is stored locally and can be accessed at:
- `~/Library/Application Support/AmpereBuddy/`

### Data Deletion
You can delete all app data:
1. In Settings > System, use "Clear History" and "Clear Alerts Log"
2. Or delete the folder: `~/Library/Application Support/AmpereBuddy/`
3. To remove preferences: delete the app's plist from `~/Library/Preferences/`

### Data Portability
Your data is stored in standard JSON format and can be exported or backed up at any time.

---

## Children's Privacy

AmpereBuddy does not collect any personal information and is suitable for users of all ages.

---

## Changes to This Policy

We may update this privacy policy occasionally. Changes will be noted with an updated "Last updated" date at the top of this document.

---

## Contact

For privacy-related questions, visit [macfoundry.it/amperebuddy](https://macfoundry.it/amperebuddy).

---

## Conclusion

AmpereBuddy is designed to be a privacy-respecting application. We believe your battery data should stay on your device, and we've built the app to ensure that's exactly what happens.
